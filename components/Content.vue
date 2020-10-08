<template>
    <div class="content-wrapper">
         <div class="content-header">
            <div class="container-fluid">
                <div class="row mb-2">
                    <div class="col-sm-6">
                        <h1 class="m-0">{{title}}</h1>
                    </div>
                    <div class="col-sm-6">
                        <ol class="breadcrumb float-sm-right">
                            <li v-bind:key="k" class="breadcrumb-item" :class="k == breadcrumb.length-1 ? 'active' : ''" v-for="(item,k) in breadcrumb">
                                {{item}}
                            </li>
                        </ol>
                    </div>
                </div>
            </div>
            <section class="content">
                <slot></slot>
            </section>
        </div>
    </div>
</template>

<script>
export default {
    name: "Content",
    props:["title", "breadcrumb"],
}
</script>