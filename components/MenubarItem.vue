<template>
    <li class="nav-item">
        <a href="" class="nav-link">
            <i class="nav-icon" :class="icon"></i>
            <p>{{text}}</p>
        </a>
    </li>
</template>

<script>
export default {
    name: "MenubarItem",
    props: ["text", "icon", "href"]
}
</script>