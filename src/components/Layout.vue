<template>

<div class="header">
    <slot name="header"></slot>
</div>

<div class="resume">
    <slot name="resume"></slot>
</div>

<div class="movements">
    <div class="head">
        <div class="grip"></div>
    </div>

    <div class="body">
        <slot name="movements"></slot>
    </div>

</div>


</template>

<style>
@import '../assets/css/Layout/layout.css';
</style>