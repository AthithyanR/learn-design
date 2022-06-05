# 1. requirement calibering
  ## functional requirements:
    - user should be able to paste some data and generate a public url
    - url alive / ttl
  ## non-functional requirement:
    - database should be scalable (partioning)
    - url should be unique
    - it should have availablity
  ## analytics:
    - reads per document
  
# 2. design considerations
  - POST doc (10kb) & return uid
  - GET  doc by uid
 
 # 3. capacity estimation:
  ## traffic estimates:
    - 1 millions users.
    - average 11 writes per second.
    - average 57 reads per second.
  ## storage estimates:
    - 10 gb document per day
    - 7 mb keys per day
  ## bandwidth estimates:
    - write - 110 kb per second
    - read - 600 kb per second
  ## memory estimates:
    - 20% url needs to be cached
    - (5 million req / 20 percent) * 10kb
    
 ## 4.Defining data model:
 
 ## 5. HLD:
 
 ## 6. detailed design:
 
 ## 7. bottlenecks:
