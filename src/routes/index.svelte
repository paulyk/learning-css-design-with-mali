<script>
import Button from "$lib/components/Button.svelte";
import Header from "$lib/components/Header.svelte";
import PrimaryButton from "$lib/components/PrimaryButton.svelte";
import SecondaryButton from "$lib/components/SecondaryButton.svelte";

</script>

<Header/>

<main>
    <PrimaryButton>I am abutton yes</PrimaryButton>
    <SecondaryButton>i want snacks</SecondaryButton>
    <Button>this is he fib</Button>
    
    <hr>
    <PrimaryButton disabled={true}>I am abutton yes</PrimaryButton>
    <SecondaryButton>i want snacks</SecondaryButton>
    <Button>this is he fib</Button>
</main>