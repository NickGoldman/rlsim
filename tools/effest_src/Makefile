effest: *.py effest_preamble effest_main
	cat effest_preamble *.py effest_main > effest;chmod +x effest
com:
	git commit -a
t: effest
	@./effest -g ./expr.fas -u -v -f test/ref.fas -k test/effest_counts.pk
pt: effest
	@./effest -u -v -f ../test/ref.fas ../test/aln1.sam
clean:
	rm -f effest
