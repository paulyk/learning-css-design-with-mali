<script lang="ts">
    import Button from "./Button.svelte";
    export let disabled = false
</script>

<Button buttonType='primary' {disabled}><slot>default</slot></Button>