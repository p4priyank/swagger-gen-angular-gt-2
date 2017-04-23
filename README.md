Generate Angular 2+ providers code from swagger 2.0 schema json
------------------------------------------------------------

Set following constants inside config/app.config.params.js

    - LIST_SWAGGER_CONF_ENDPOINTS
        Specify list of providers to be generate from host + swagger shema subpath here
    - Example : 
	LIST_SWAGGER_CONF_ENDPOINTS: [{
	    'className': 'AccountApi',
	    'apiName': 'Account',
	    'url': 'http://192.168.0.1',
	    'path': '../src/common/swagger-providers/account-api.provider.ts',
	    'sub_path': '/api/account/doc?format=openapi'
	},{
	    'className': 'MessageApi',
	    'apiName': 'Message',
	    'url': 'http://192.168.0.1',
	    'path': '../src/common/swagger-providers/message-api.provider.ts',
	    'sub_path': '/api/message/doc?format=openapi'
	}]
