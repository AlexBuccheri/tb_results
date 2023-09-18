Copying files from Output Directory
------------------------------------

input_dir=/Users/alexanderbuccheri/Codes/tb_benchmarking/outputs/tblite1/e_vs_v
output_dir=/Users/alexanderbuccheri/Codes/tb_outputs/tblite1/e_vs_v

dirs=("bn_cubic" "copper" "gan" "mgo" "pbs" "tio2_ana" "ws2" "bn_hex" "diamond" "germanium" "mos2" "pbte" "tio2_rutile" "zinc_oxide" "cdse" "gaas" "graphite" "nacl" "silicon" "wo3_monoclinic" "zro2"); for dir in "${dirs[@]}"; do cp "$input_dir/$dir/e_vs_v.dat" "$output_dir/e_vs_v_$dir.dat"; done
