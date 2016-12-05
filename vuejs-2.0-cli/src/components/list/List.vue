<template>
    <div class="list">
        <div class="am-panel am-panel-default">
            <div class="am-panel-hd">
                <h3 class="am-panel-title">创悦保险列表 {{todoCount}}</h3>
            </div>
            <div class="am-panel-bd">
                <form class="am-form" v-on:submit.prevent="addTodo(newTodo)">
                        <div class="am-form-group">
                            <input type="text" class="am-form-field" placeholder="输入保险名称" v-model="newTodo.title">
                            <button type="submit" class="am-btn am-btn-primary am-btn-block">提交</button>
                        </div>
                </form>
            </div>
            <ul class="am-list am-list-static am-list-border">
                <li v-for="(todo,index) in todos">
                        <button class="am-badge am-badge-danger" v-on:click="deleteTodo(index)">Del</button>
                    <a href="#">{{todo.title}}</a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {

    name: 'list',

    data(){
      return{
          todos:[
              {id:1,title:'平安保险'}
          ],
          newTodo:{id:null,title:''}
      }
    },

    computed:{
        todoCount(){
            return this.todos.length;
        }
    },

    methods:{
        addTodo(newTodo)
        {
            this.todos.push(newTodo),
                this.newTodo ={id:null,title:''}
        },
        deleteTodo(index){
            this.todos.splice(index,1)
        }
    }

};
</script>

<style>
</style>
