transcript on
if {[file exists rtl_work]} {
	vdel -lib rtl_work -all
}
vlib rtl_work
vmap work rtl_work

vlog -sv -work work +incdir+C:/2025_summer/SOC_Mini_GPU/Mini_GPU {C:/2025_summer/SOC_Mini_GPU/Mini_GPU/alu.sv}
vlog -sv -work work +incdir+C:/2025_summer/SOC_Mini_GPU/Mini_GPU {C:/2025_summer/SOC_Mini_GPU/Mini_GPU/decoder.sv}
vlog -sv -work work +incdir+C:/2025_summer/SOC_Mini_GPU/Mini_GPU {C:/2025_summer/SOC_Mini_GPU/Mini_GPU/fetcher.sv}
vlog -sv -work work +incdir+C:/2025_summer/SOC_Mini_GPU/Mini_GPU {C:/2025_summer/SOC_Mini_GPU/Mini_GPU/lsu.sv}
vlog -sv -work work +incdir+C:/2025_summer/SOC_Mini_GPU/Mini_GPU {C:/2025_summer/SOC_Mini_GPU/Mini_GPU/pc.sv}
vlog -sv -work work +incdir+C:/2025_summer/SOC_Mini_GPU/Mini_GPU {C:/2025_summer/SOC_Mini_GPU/Mini_GPU/scheduler.sv}
vlog -sv -work work +incdir+C:/2025_summer/SOC_Mini_GPU/Mini_GPU {C:/2025_summer/SOC_Mini_GPU/Mini_GPU/core.sv}
vlog -sv -work work +incdir+C:/2025_summer/SOC_Mini_GPU/Mini_GPU {C:/2025_summer/SOC_Mini_GPU/Mini_GPU/dcr.sv}
vlog -sv -work work +incdir+C:/2025_summer/SOC_Mini_GPU/Mini_GPU {C:/2025_summer/SOC_Mini_GPU/Mini_GPU/dispatch.sv}
vlog -sv -work work +incdir+C:/2025_summer/SOC_Mini_GPU/Mini_GPU {C:/2025_summer/SOC_Mini_GPU/Mini_GPU/registers.sv}
vlog -sv -work work +incdir+C:/2025_summer/SOC_Mini_GPU/Mini_GPU {C:/2025_summer/SOC_Mini_GPU/Mini_GPU/gpu.sv}
vlog -sv -work work +incdir+C:/2025_summer/SOC_Mini_GPU/Mini_GPU {C:/2025_summer/SOC_Mini_GPU/Mini_GPU/controller.sv}

vlog -sv -work work +incdir+C:/2025_summer/SOC_Mini_GPU/Mini_GPU {C:/2025_summer/SOC_Mini_GPU/Mini_GPU/gpu_tb.sv}

vsim -t 1ps -L altera_ver -L lpm_ver -L sgate_ver -L altera_mf_ver -L altera_lnsim_ver -L fiftyfivenm_ver -L rtl_work -L work -voptargs="+acc"  testbench

add wave *
view structure
view signals
run -all
