Idrizoski Elmir 126004
SI_2022_lab2_126004
![CFG_lab2](https://user-images.githubusercontent.com/6106051/171959711-4d48d0e1-9fb7-45a2-8312-c785cdd3af65.png)
Цикломатската комплексност на овој код се одредува според тоа каде се носат одлуки, односно if-ифови и for цикслуси.  IF-ифови има 7 и има еден фор циклус и на овие  се додава плус еден. 7+1+1=9 
Или според полињата од CFG на сликата има 8 и еден надворешен 8+1=9.

C0 – EveryStatemant					C1 – EveryBranch
C1	[ ]	[0,#,0]	[0,#,0,#,0,#,0,#,# ]
1-2	*		
1-3.4.5		*	
3,4,5-6		*	
3.4.5-7,8			*
8,8a-9			*
9-21			*
9-10			*
21-22			*
22-8b			*
10-11			*
11-12			*
11-16			*
12-13			*
12-14			*
13-20			*
14-15			*
15-20			*
16-17			*
17-20			*
16-18			*
18-19			*
18-20			*
19-20			*
20-8b			*
8b-8a			*
8a-23			*

C0	[ ]	[0,#,0]	[0,#,0,#,0,#,0,#,# ]
1	*		
2	*		
3		*	
4		*	
5		*	
6		*	
7			*
8			*
9			*
10			*
11			*
12			*
13			*
14			*
15			*
16			*
17			*
18			*
19			*
20			*
21			*
22			*
23			*


	



имаме три теста за вој код. Со првиот тест празна листа се поминуваат 1, 2 јазол каде се фрла исклуцок за празна листа исто така поминува и низ бранчот 1-2.
Со вториот тест се поминува низ  јазлите 3456 и бранчовите 1-345, 345-6, каде што се фрла и вторит исклучок за кодот. 
Со третиот тест се поминува низ останатите јазли и бранчови каде што поминува успешно.

