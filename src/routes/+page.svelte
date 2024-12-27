<script lang="ts">
    import Component from '$lib/component.svelte';
    import Component1 from '$lib/component1.svelte';
</script>

<h1>Bug reproduction</h1>

<!-- This breaks on hydration -->
<Component1>
    <svelte:fragment slot="left">
        <div class="mx-auto lg:mx-0">
            <Component>
                For a given location you get a condensed overview, you can use as an identifer of
                red flags and easy benchmarking:

                <ul class="ml-10 mt-6 list-disc text-start">
                    <li>Overall risk score</li>
                    <li>Earthquake</li>
                    <li>Storm</li>
                    <li>Flood</li>
                </ul>
            </Component>
        </div>
    </svelte:fragment>
</Component1>
