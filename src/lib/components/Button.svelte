<script context="module" lang="ts">
    export type ButtonType = 'primary' | 'secondary' | 'default'
</script>

<script lang="ts">
    export let buttonType:ButtonType = 'default'
    export let disabled = false
</script>

<button 
    class={`btn ${buttonType}`}
    class:disabled={disabled}    
>
    <slot/>
</button>

<style>
    .btn {
        cursor: pointer;
        font-family: inherit;
        font-size: inherit;
        padding: 1rem;
    }

    .primary {
        background: rgb(101, 195, 190);
        color: rgb(7, 38, 81);
    }

    .secondary {
        background: gainsboro;
        color: #333;
    }

    .default {
        background: white;
        color: maroon;
    }

    .disabled {
        opacity: 0.5;
        cursor: not-allowed;
    }
</style>