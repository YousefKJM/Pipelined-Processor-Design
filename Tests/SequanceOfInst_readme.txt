	AND $0, $0, $0 ;
	CAND $1, $0, $1;
	OR $1, $1, $0;
	XOR $1, $1, $1 ;
	ADD $2, $0, $1;
	NADD $3, $2, $1;
	SLT $4, $2, $1;
	SLTU $4, $1, $3;
	ANDI $4, $0, 5;
	CANDI $3, $1, 3;
	ORI $5, $5, 15;
	XORI $4, $4, 1;
	ADDI $1, $1, 8;
	NADDI $0, $0, 10;
	SLTI $4, $0, 2;
	SLTUI $4, $0, 5;
	SLL $3, $0, 2;
	SRL $4, $0, 2;
	SRA $3, $0, 2;
	ROR $4, $0, 5;
	SW $3, 0($1)
	LW $0, 0($1) 
	BEQZ $5, label1;
	BNEZ $3, label2;
	BLTZ $1, label3;
	BGEZ $2, label4;
	BGTZ $2, label5;
	BLTZ $4, label6;
label1:	SET 1 ;
	JR $7, 0;
label2:	SET 2 ;
	JR $7, 0;
label3:	SET 3 ;
	JR $7, 0;
label4:	SET 4 ;
	JR $7, 0;
label5:	SET 5 ;
	JR $7, 0;
label6:	SET 6 ;
	JALR $7, 0;
	SET 5;
	SSET 7; 
	JAL procedure;
	addi $2, $2, 4
procedure:	addi $2, $2, 7
	J next ;
	addi $1, $6, 3
next:	addi $1, $6, 4