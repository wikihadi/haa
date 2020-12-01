<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-12">
                <div class="card">
                    <div class="card-header">Example Component</div>

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
        
        mounted() {
           var dataToSend = {
	"method" : "login",
	"input_type" : "JSON",
	"response_type" : "JSON"
};
var restData = {
	user_auth : {
		user_name : "DemoUser",
		password : "b57014dd3a80639cc4390294a0218401"
	},
	application : "TEST",
	name_value_list : {
		"name" : "language",
		"value" : "fa_IR"
	},
	"meta_data":true,
};


        }
    }
</script>
