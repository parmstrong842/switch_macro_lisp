(setf x 1 y 2)
2

(select (+ y x)
    (when (2 4 6 8)
        (print "even")
        (* y 4)
    )
    (when (1 3 5 7)
        (print "odd")
        (+ (* y 4) 1)
    )
    (default
        (print "default")
        y
    )
)
"odd"
9

(setf x 2 y 4)
4

(select (+ y x)
    (when (2 4 6 8)
        (print "even")
        (* y 4)
    )
    (when (1 3 5 7)
        (print "odd")
        (+ (* y 4) 1)
    )
    (default
        (print "default")
        y
    )
)
"even"
16

(setf x 10 y 10)
10

(select (+ y x)
    (when (2 4 6 8)
        (print "even")
        (* y 4)
    )
    (when (1 3 5 7)
        (print "odd")
        (+ (* y 4) 1)
    )
    (default
        (print "default")
        y
    )
)
"default"
10