.PHONY: all clean

all: volume_meter record play duplex

volume_meter: volume_meter.hs
	ghc -threaded --make -package alsa -o $@ $<

record: record.hs
	ghc -threaded --make -package alsa -o $@ $<

play: play.hs
	ghc -threaded --make -package alsa -o $@ $<

duplex: duplex.hs
	ghc -threaded --make -package alsa -o $@ $<

clean:
	-rm -f *o *.hi
	-rm -f volume_meter record play duplex