routes.get ( '/', ( request, response ) => {
	return response.send (
		"Hello World"
	)
} )

routes.get ( '/query', ( request, response ) => {
	const params = request.query

	console.log ( params )
	return response.json ( {
		msg: "Hello World"
	} )
} )

routes.get ( '/route/:id', ( request, response ) => {
	const params = request.params

	console.log ( params )
	return response.json ( {
		msg: "Hello World"
	} )
} )

routes.post ( '/request', ( request, response ) => {
	const params = request.body

	console.log ( params )
	return response.json ( {
		msg: "Hello World"
	} )
} )


routes.post ( '/users', ( request, response ) => {
	return response.json ( {
		msg: "Hello World"
	} )
} )

