# r-assignment
## Put comments here that give an overall description of what your
	## functions do
	

	## Write a short comment describing this function
	

	# Creates  special matrix object that can cache its inverse 
	

	makeCacheMatrix <- function(x = matrix()) {
	  inv <- NULL
	  set <- function(y){
	    x <<- y
	    y <<- NULL
	  }
	get <- function()x
	setinverse <- function(inverse) inv <<- inverse
	getinverse <- function() inv
	list(set = set, get = get, setinverse = setinverse, getinverse = getinverse)
	}
	

	

	## Write a short comment describing this function
	

	##This a function which computes the inverse of the special "matrix" 
	## returned by makeCacheMatrix. If the inverse has already been calculated, 
	## then the cachesolve should retrieve the inverse from the cache
	

	

	cacheSolve <- function(x, ...) {
