<script lang="ts">
  

</script>

<div>
    <div class="flex flex-col items-center lg:items-start lg:pr-4">
        <div>
            <slot name="above-title" />
        </div>
        <div
            class="mt-6 text-center text-3xl font-semibold text-gray-900 dark:text-gray-50 md:text-4xl lg:text-left">
        </div>
        <p
            class="mt-2 max-w-lg text-center text-xl leading-snug tracking-wide text-gray-800 dark:text-gray-200 lg:mt-5 lg:text-start">
            <slot />
        </p>
       
    </div>
</div>


