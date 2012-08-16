zip: \
		lx9-PCB_Edges.gbr \
		lx9.drl \
		lx9-NPTH.drl \
		lx9-SilkS_Front.gto \
		lx9-Mask_Front.gts \
		lx9-Front.gtl \
		lx9-GND.gbr \
		lx9-3.3V.gbr \
		lx9-Back.gbl \
		lx9-Mask_Back.gbs \
		lx9-SilkS_Back.gbo \
		README
	zip makestuff-lx9-v1.0.zip $+

front: lx9-PCB_Edges.gbr lx9.drl lx9-NPTH.drl lx9-SilkS_Front.gto lx9-Mask_Front.gts lx9-Front.gtl
	gerbv --export=png --antialias --dpi=1200 --background=#284907 -o front.png \
		lx9-PCB_Edges.gbr   --foreground=#FFFFFFFF \
		lx9.drl             --foreground=#000000FF \
		lx9-NPTH.drl        --foreground=#000000FF \
		lx9-SilkS_Front.gto --foreground=#FFFFFF80 \
		lx9-Mask_Front.gts  --foreground=#88888880 \
		lx9-Front.gtl       --foreground=#676315FF
	firefox front.png

back: lx9-PCB_Edges.gbr lx9.drl lx9-NPTH.drl lx9-SilkS_Back.gbo lx9-Mask_Back.gbs lx9-Back.gbl
	gerbv --export=png --antialias --dpi=1200 --background=#284907 -o back.png \
		lx9-PCB_Edges.gbr   --foreground=#FFFFFFFF \
		lx9.drl             --foreground=#000000FF \
		lx9-NPTH.drl        --foreground=#000000FF \
		lx9-SilkS_Back.gbo --foreground=#FFFFFF80 \
		lx9-Mask_Back.gbs  --foreground=#88888880 \
		lx9-Back.gbl       --foreground=#676315FF
	convert back.png -flop back.png
	firefox back.png

clean: FORCE
	rm -f *.png *.zip

FORCE:
