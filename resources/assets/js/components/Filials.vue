<template>
<div>
    <div class="filials" v-for="(item, key) in filials" v-bind:key="item.key" :filter-key="filterKey"> 
        <h3>
            {{ key }} <small></small>
        </h3>

        <groups :filter-key="filterKey" 
          :group-selected="groupSelected" 
          :groups="item"
        >
        </groups>
    </div>

</div>
</template>

<script>
    export default {
        props: [
            'filterKey',
            'filialSelected',
            'groupSelected',
            'phones', 
            'groups', 
            'filials'
        ],
        methods: {
        },
        computed: {
        }
    }
</script>