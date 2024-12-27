<script lang="ts">
  import Component from "$lib/component.svelte";
  import Component1 from "$lib/component1.svelte";
</script>

<h1>Bug reproduction</h1>

<!-- This breaks on hydration -->
<Component1>
  <svelte:fragment slot="slotA">
    <Component>
      some text without any element around it

      <ul>
        <li>Overall risk score</li>
      </ul>
    </Component>
  </svelte:fragment>
</Component1>
