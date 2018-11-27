all: histogram.png report.html letters_freq.png

clean:
	rm -f words.txt histogram.tsv histogram.png report.html

histogram.tsv: histogram.r words.txt
	Rscript $<
	
histogram.png: histogram.tsv
	Rscript -e 'library(ggplot2); qplot(Length, Freq, data=read.delim("$<")); ggsave("$@")'
	rm -f Rplots.pdf
	
report.html: report.rmd histogram.tsv histogram.png
	Rscript -e 'rmarkdown::render("$<")'
	
letters_freq.png: letters_freq.tsv
	Rscript -e 'library(ggplot2); ggplot(data=read.delim("$<"), aes(x=letter, y=frequency)) + geom_bar(stat = "identity", fill= "plum"); ggsave("$@")'
	rm Rplots.pdf
	
letters_freq.tsv: letters_freq.r words.txt
	Rscript $<

words.txt: /usr/share/dict/words
	cp $< $@

# words.txt:
#	Rscript -e 'download.file("http://svnweb.freebsd.org/base/head/share/dict/web2?view=co", destfile = "words.txt", quiet = TRUE)'
