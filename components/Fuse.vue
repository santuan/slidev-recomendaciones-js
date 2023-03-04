<script setup lang="ts">
import { computed, ref, watch } from 'vue'
import type { UseFuseOptions } from './team'
import { useFuse } from '@vueuse/integrations/useFuse'

interface DataItem {
  firstName: string
  lastName: string
}

const data = ref<DataItem[]>([
  {
    firstName: 'Roslyn',
    lastName: 'Mitchell',
  },
  {
    firstName: 'Cathleen',
    lastName: 'Matthews',
  },
  {
    firstName: 'Carleton',
    lastName: 'Harrelson',
  },
  {
    firstName: 'Allen',
    lastName: 'Moores',
  },
  {
    firstName: 'John',
    lastName: 'Washington',
  },
  {
    firstName: 'Brooke',
    lastName: 'Colton',
  },
  {
    firstName: 'Mary',
    lastName: 'Rennold',
  },
  {
    firstName: 'Nanny',
    lastName: 'Field',
  },
  {
    firstName: 'Chasity',
    lastName: 'Michael',
  },
  {
    firstName: 'Oakley',
    lastName: 'Giles',
  },
  {
    firstName: 'Johanna',
    lastName: 'Shepherd',
  },
  {
    firstName: 'Maybelle',
    lastName: 'Wilkie',
  },
  {
    firstName: 'Dawson',
    lastName: 'Rowntree',
  },
  {
    firstName: 'Manley',
    lastName: 'Pond',
  },
  {
    firstName: 'Lula',
    lastName: 'Sawyer',
  },
  {
    firstName: 'Hudson',
    lastName: 'Hext',
  },
  {
    firstName: 'Alden',
    lastName: 'Senior',
  },
  {
    firstName: 'Tory',
    lastName: 'Hyland',
  },
  {
    firstName: 'Constance',
    lastName: 'Josephs',
  },
  {
    firstName: 'Larry',
    lastName: 'Kinsley',
  },
])

const search = ref('')
const filterBy = ref('both')
const keys = computed(() => {
  if (filterBy.value === 'first')
    return ['firstName']
  else if (filterBy.value === 'last')
    return ['lastName']
  else return ['firstName', 'lastName']
})

const resultLimit = ref<number | undefined>(undefined)
const resultLimitString = ref<string>('')
watch(resultLimitString, () => {
  if (resultLimitString.value === '') {
    resultLimit.value = undefined
  }
  else {
    const float = parseFloat(resultLimitString.value)
    if (!isNaN(float)) {
      resultLimit.value = Math.round(float)
      resultLimitString.value = resultLimit.value.toString()
    }
  }
})

const exactMatch = ref(false)
const isCaseSensitive = ref(false)
const matchAllWhenSearchEmpty = ref(true)

const options = computed<UseFuseOptions<DataItem>>(() => ({
  fuseOptions: {
    keys: keys.value,
    isCaseSensitive: isCaseSensitive.value,
    threshold: exactMatch.value ? 0 : undefined,
  },
  resultLimit: resultLimit.value,
  matchAllWhenSearchEmpty: matchAllWhenSearchEmpty.value,
}))

const { results } = useFuse(search, data, options)
</script>




<template>
  <div class="mx-auto w-full mt-6">
    <input v-model="search" placeholder="Buscar por nombre..." type="text"
      class="text-gray-100 border-2 border-gray-500 rounded-lg w-full mb-4 p-2">
    <div class="flex flex-wrap">
      <div class="rounded relative  flex items-center">
        <select v-model="filterBy"
          class="p-2 text-gray-100 border-2 rounded-lg border-gray-500 bg-transparent">
          <option value="both">
            Nombre y apellido
          </option>
          <option value="first">
            Nombre
          </option>
          <option value="last">
            Apellido
          </option>
        </select>
      </div>
      <span class="flex-1" />
      <div class="flex flex-row flex-wrap gap-x-4">
        <label class="checkbox">
          <input v-model="exactMatch" type="checkbox" class="accent-red-600">
          <span>Exact Match</span>
        </label>
        <label class="checkbox">
          <input v-model="isCaseSensitive" type="checkbox" class="accent-red-600">
          <span>Case Sensistive</span>
        </label>
        <label class="checkbox">
          <input v-model="matchAllWhenSearchEmpty" type="checkbox" class="accent-red-600">
          <span>Match all when empty</span>
        </label>
      </div>
    </div>
  </div>
  <div class="mt-4 mx-auto w-full h-64 text-sm overflow-y-auto">
    <template v-if="results.length > 0">
      <div v-for="result in results" :key="result.item.firstName + result.item.lastName" class="py-2">
        <div class="flex flex-col">
          <span>
            {{ result.item.firstName }} {{ result.item.lastName }}
          </span>
          <span class="text-sm opacity-50">
            Score Index: {{ result.refIndex }}
          </span>
        </div>
      </div>
    </template>
    <template v-else>
      <div text-center pt-8 pb-4 opacity-80>
        sin resultados
      </div>
    </template>
  </div>
</template>


<style scoped>

.checkbox {
  @apply inline-flex items-center my-auto cursor-pointer select-none;
}

select {
  @apply bg-white text-gray-900
}

.checkbox input {
  appearance: none;
  padding: 0;
  display: inline-block;
  vertical-align: middle;
  background-origin: border-box;
  user-select: none;
  flex-shrink: 0;
  height: 1rem;
  width: 1rem;
  @apply bg-gray-400/30;
  @apply rounded-md h-4 w-4 select-none;
}

.checkbox input:checked {
  background-image: url("data:image/svg+xml,%3csvg viewBox='0 0 16 16' fill='white' xmlns='http://www.w3.org/2000/svg'%3e%3cpath d='M12.207 4.793a1 1 0 010 1.414l-5 5a1 1 0 01-1.414 0l-2-2a1 1 0 011.414-1.414L6.5 9.086l4.293-4.293a1 1 0 011.414 0z'/%3e%3c/svg%3e");
}

.checkbox span {
  @apply ml-1.5 text-13px opacity-70;
}
</style>