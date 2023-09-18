Copying from the main project:
-------------

To do for 4,4,4 or 8,8,8 just modify input and output dirs

input_dir=/Users/alexanderbuccheri/Codes/tb_benchmarking/outputs/tblite1/x23_e_vs_v/1_1_1
output_dir=/Users/alexanderbuccheri/Codes/tb_outputs/tblite1/x23_e_vs_v/1_1_1

dirs=("CO2" "benzene" "hexamine" "oxacb" "trioxane" "ammonia" "ethcar" "naph" "succinic" "acetic" "cyanamide" "hexdio" "pyrazine" "triazine" "adaman" "cytosine" "imdazole" "oxaca" "pyrazole" "urea"); for dir in "${dirs[@]}"; do if [[ $dir != *_g ]]; then cp "$input_dir/$dir/e_vs_v.dat" "$output_dir/e_vs_v_$dir.dat"; fi; done
