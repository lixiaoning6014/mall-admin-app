<!--  -->
<template>
    <div class="main-header">
        <a-button type="primary" style="margin-bottom: 16px" @click="toggleCollapsed">
            <a-icon :type="collapsed ? 'menu-unfold' : 'menu-fold'" />
        </a-button>
        <div class="breadcrumb">
            <Breadcrumb>
                <Breadcrumb.Item>首页</Breadcrumb.Item>
                <Breadcrumb.Item>
                    <a href="">统计</a>
                </Breadcrumb.Item>
            </Breadcrumb>
        </div>
        <ul class="user-info">
            <li>欢迎XXXXX
                <a-icon type="down" />
            </li>
            <li>退出</li>
        </ul>
    </div>
</template>

<script>
    export default {
        data() {
            return {}
        }
    }
</script>

<style lang='scss'>

</style>