<script lang="ts">
    import Register from "./Register.svelte"

    // If you uncomment all the below code, flickering will not happen.
    // However, this seems like more of a workaround than a solution.
    
    // import { onMount } from "svelte";

    // let ready = false;

    // onMount(() => {
    //     ready = true;
    // });
</script>

<!-- {#if ready} -->
<Register>
    <div slot="top">
        <p class="text-center">
            This is a test sentence. It should not flicker.
            <br />
            However, it blinks from gray to green, and from center to left.
        </p>
    </div>
</Register>

<!-- {/if} -->
<style>
    .text-center {
        text-align: center;
    }
</style>
