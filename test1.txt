(define fib (lambda (n) (if (< n 2) 1 (+ (fib (- n 1)) (fib (- n 2))))))
(define range (lambda (a b) (if (= a b) (quote ()) (cons (fib a) (range (+ a 1) b)))))
(range 0 10)