1. 
	To reproduce:
		book the Canon DSLR Camera from Jan 9 to Jan 16 to over lap the existing booking

	Explain one fix
		I change it logical operator "and" is now use, end_a parameter is used.
		instead of using greater than and less than only we use greaterthan equal to and less than
		equal to so that even start_b and star_b is the same and end_b and end_a is the same we can
		still catch eh over lapping dates between dates.
	

	Show the failure
		it did not use the paramer end_a and logical operator "and"
		start_b <= start_a <= end_b 

	wrongly allowed
		the statement is allowed but totally wrong because it didnt logical operator "and" to filter
		between from and to dates also the use of greater than and less than is wrong

		start_b <= start_a <= end_b

	AI use
		I use Gemini to fix
		How I check is  the existing data dates is from Jan 10 To Jan 15
		swallows Old  that is 		Jan 01 – Jan 17
		overlaps Start that is 		Jan 05 – Jan 12
		overlaps End that is 		Jan 12 – Jan 20
		New completely inside Old	Jan 11 – Jan 14

