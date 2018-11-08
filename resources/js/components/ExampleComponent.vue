<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-8">
                <div class="card card-default">
                    <div class="card-header">aaaaaab</div>

                    <div class="card-body">
                       <ul>
                           <li v-for="thought in thoughts" :key="thought.birth_year">
                               {{thought.name}}
                           </li>
                       </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data(){
            return{
                thoughts:[]
            }
			
        },
        created: function(){
              this.$http.get('https://swapi.co/api/people/1').then(function(response){
               thoughts = response.body; 
           }, function(){
              alert('Error!');
           });
        }
    }
</script>
