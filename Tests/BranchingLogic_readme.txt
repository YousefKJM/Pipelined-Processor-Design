     addi	$3, $2, 6	; 
        beqz	$6,  do	; 
        addi	$6, $5, 6	; 
do:	    sll	    $1, $3, 2		;
        j next ;
        addi $4, $2, 4 ;
next:   addi $4, $2, 10 ;