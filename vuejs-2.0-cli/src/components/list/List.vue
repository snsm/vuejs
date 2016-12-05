<template>
    <div class="list">
        <div class="am-panel am-panel-default">
            <div class="am-panel-hd">
                <h3 class="am-panel-title">创悦保险列表</h3>
            </div>
            <div class="am-panel-bd">
                <form class="am-form">
                        <div class="am-form-group">
                            <input type="text" class="am-form-field" placeholder="输入保险名称">
                            <button type="submit" class="am-btn am-btn-primary am-btn-block">提交</button>
                        </div>
                </form>
            </div>
            <ul class="am-list am-list-static am-list-border">
                <li>
                    <span class="am-badge am-badge-success">YES</span> <span class="am-badge am-badge-danger">NO</span>
                    <a href="#">人保保险</a>
                </li>
                <li>
                    <span class="am-badge am-badge-success">YES</span> <span class="am-badge am-badge-danger">NO</span>
                    <a href="#">人保保险</a>
                </li>
                <li>
                    <span class="am-badge am-badge-success">YES</span> <span class="am-badge am-badge-danger">NO</span>
                    <a href="#">人保保险</a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
  name: 'list'
};
</script>

<style>
</style>
