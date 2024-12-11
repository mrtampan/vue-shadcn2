<script setup>
import { cn } from "@/lib/utils";
import { badgeVariants } from ".";

defineProps({
    variant: {
        type: String,
        default: "default",
    },
    size: {
        type: String,
        default: "default",
    },
    as: {
        type: String,
        default: "badge",
    },
});
</script>

<template>
  <component
    :is="as"
    :class="cn(badgeVariants({ variant, size }), $attrs.class ?? '')"
  >
    <slot />
  </component>
</template>
