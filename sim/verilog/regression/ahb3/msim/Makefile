all: build

build:
	@if [ ! -e work ]; then vlib work; fi
	@vlog -sv +incdir+../../../../../rtl/verilog/ahb3/pkg -f system.vc
	vsim -c -do run.do work.mpsoc_spram_testbench
