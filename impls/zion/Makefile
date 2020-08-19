#####################

SRCS = $(shell find . -regex '\./step.*\.zion')
BINS = $(SRCS:%.zion=%)

#####################

all: $(BINS)

$(BINS): $(shell find . -regex '\./.*\.zion')
	zion build $@

clean:
	-rm $(BINS)
