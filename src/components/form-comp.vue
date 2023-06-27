<template>
    <h2>Text Input</h2>

<input v-model="text">{{ text }}

<h2>Checkbox</h2>

<input type="checkbox" id="checkbox" v-model="checked">

<label for="checkbox">checked{{ checked }}</label>

<h2>Multi Checkbox</h2>
    <input type="checkbox" id="cheslyn" v-model="checkedName" value="cheslyn">
    <label for="cheslyn">cheslyn</label>

    <input type="checkbox" id="luke" v-model="checkedName" value="luke">
    <label for="luke">luke</label>

    <p>
        <pre>
            {{ checkedName }}
        </pre>
    </p>

    <h2>Radio</h2>

    <input type="radio" id="one" value="one" v-model="picked">
    <label for="one">One</label>
    <br>
    <input type="radio" id="two" value="two" v-model="picked">
    <label for="two">Two</label>
    <br>
    <span>Picked: {{ picked }}</span>

    <h2>Multi Select</h2>

    <select v-model="multiSelected" multiple style="width: 100px">
        <option>A</option>
        <option>B</option>
        <option>C</option>
    </select>
    <span>Selected {{ multiSelected }}</span>
</template>

<script>
    export default {
        data() {
            return {
                text: '',
                checked: true,
                checkedName: ['cheslyn'],
                picked: 'one',
                multiSelected: ['A']
            }
        }
    };
</script>
