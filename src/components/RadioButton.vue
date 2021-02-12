<template>
    <div>
        <input type="radio" name="animal" :id=animal.id :value=animal.name>
        <label :for=animal.id>{{ animal.name }}</label>
    </div>
</template>

<script>
export default {
    name: 'RadioButton',
    props: ['animal']
}
</script>