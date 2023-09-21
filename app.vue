<script lang="ts" setup>
import { collection } from 'firebase/firestore';

const firestore = useFirestore();

const { data } = useCollection(collection(firestore, 'test'));
</script>

<template>
  <div>
    {{ data }}
  </div>
</template>
