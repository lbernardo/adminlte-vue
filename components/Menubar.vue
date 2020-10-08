<template>
    <nav class="mt-2">
        <ul class="nav nav-pills nav-sidebar flex-column" data-widget="treeview" role="menu" data-accordion="false">
            <slot></slot>
        </ul>
    </nav>
</template>
<script>
export default {
    name: "Menubar"
}
</script>