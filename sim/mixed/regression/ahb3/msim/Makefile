all: build

build:
	@if [ ! -e work ]; then vlib work; fi
	@vlog -sv +incdir+../../../../../rtl/verilog/ahb3/pkg -f system.verilog.vc
	@vcom -2008 -f system.vhdl.vc
	vsim -c -do run.do work.mpsoc_spram_testbench
