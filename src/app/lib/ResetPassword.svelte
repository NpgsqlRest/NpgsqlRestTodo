<script lang="ts">
    // import Mail from "lucide-svelte/icons/mail";

    // // import { authLogin } from "$api/authApi";
    // // import user from "$lib/user";
    // // import getAnalyticsData from "$lib/analyticsData";

    // let emailInput: HTMLInputElement;

    // let emailMsg = $state<string>();
    // let working = $state(false);
    // //let success = $state<boolean | undefined>();


    // async function reset() {
    //     passwordMsg = undefined;
    //     emailMsg = undefined;
    //     success = undefined;

    //     if (!emailInput.value) {
    //         emailMsg = 'Email is required';
    //         emailInput.focus();
    //         return;
    //     }
    //     if (!passwordInput.value) {
    //         passwordMsg = 'Password is required';
    //         passwordInput.focus();
    //         return;
    //     }
    //     working = true;
    //     const result = await authLogin({
    //         username: emailInput.value,
    //         password: passwordInput.value,
    //         analyticsData: JSON.stringify(getAnalyticsData())
    //     });
    //     working = false;
    //     if (result.status === 200) {
    //         success = true;
    //         user.set(JSON.parse(result.response));
    //     } else {
    //         success = false;
    //         setTimeout(() => {
    //             emailInput.focus();
    //             emailInput.select();
    //             passwordInput.value = "";
    //         }, 0);
    //     }
    // }
</script>

<!-- <div class="form-control">
    <label class="label pb-0.75" class:text-error={emailMsg} for="email">
        <span class="label-text">{emailMsg ?? "Email"}</span>
    </label>
    <label class="input input-bordered flex items-center gap-2" class:input-error={emailMsg} class:input-primary={!emailMsg}>
        <Mail size="16" class="h-4 w-4 opacity-70" />
        <input 
            id="email" 
            type="email" 
            placeholder="email" 
            class="grow" 
            bind:this={emailInput} 
            disabled={working} 
            onkeypress={e => {if (e.key == "Enter"){passwordInput.focus(); passwordInput.select()}}} 
        />
    </label>
</div> -->

<!-- <button class="btn btn-primary mt-1" onclick={reset} aria-label="Login" disabled={working}>
    {#if working}
        <span class="loading loading-bars loading-xs"></span>
    {:else}
        Send Reset Link
    {/if}
</button> -->

<style lang="scss">
    .label-text {
        white-space: break-spaces;
        text-align: justify;
    }
</style>