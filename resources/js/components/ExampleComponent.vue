<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-8">
                <div class="card card-default">
                    <div class="card-header">aaaaaa</div>

                    <div class="card-body">
                        I'm an example component.
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data:{
			pokemon: []
		},
        mounted() {
            /*this.$http.get('http://pokeapi.co/api/v2/pokemon/').then(response => { 
                pokemon = response.body; 
            }, response => { 
                alert('Error'); 
            });*/
        }
    }
</script>
