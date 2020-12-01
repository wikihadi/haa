<template>
    <div class="container">
     <div class="row justify-content-center">
        <div class="col-md-12">
            <div class="card">
                <div class="card-header text-right">
                    <div class="btn-group float-right" role="group" aria-label="Basic example">
                        <button type="button" class="btn btn-secondary" v-on:click="list=true">Left</button>
                        <button type="button" class="btn btn-secondary" v-on:click.prevent="list=false">Middle</button>
                        <!-- <button type="button" class="btn btn-secondary">Right</button> -->
                    </div>
                </div>

                <div class="card-body">

        <form v-show="!list">
            <div class="form-group">
                <label>{{title}}</label>
                <input type="text" v-model="title" v-on:change.prevent="list=false" class="form-control" placeholder="Title">
                <!-- <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small> -->
            </div>
            <!-- <div class="form-group">
                <label>Date</label>
                <input type="date" class="form-control">
            </div> -->
            <!-- <div class="form-check">
                <input type="checkbox" class="form-check-input">
                <label class="form-check-label" for="exampleCheck1">Check me out</label>
            </div> -->
            <button type="submit" class="btn btn-primary">Submit</button>
        </form>

                    
                </div>
            </div>
        </div>
    </div>                               



    </div>
</template>

<script>
    export default {
  data: function () {
    return {
      title: '',
      list:true
    }
  },
        
    };


</script>
