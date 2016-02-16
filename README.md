# php_hei_strnum
php 任意进制数转换函数 支持特大数据

	$t = microtime(1);

	for ($i=0; $i < 10000; $i++) {
		$m2n_convert = hei_m2n(array('mvalue'=>'100000000000000000000000000000062','m'=>10,'n'=>64));
	}

	var_dump(microtime(1)-$t,$m2n_convert);


	// float(2.9181671142578)
	// array(6) {
	//   ["strnum"]=>
	//   string(18) "JkBMr1MuMixu40000|"
	//   ["from"]=>
	//   int(10)
	//   ["to"]=>
	//   int(64)
	//   ["strlist"]=>
	//   string(64) "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz|~"
	//   ["old_strnum"]=>
	//   string(33) "100000000000000000000000000000062"
	//   ["rmd"]=>
	//   string(1) "J"
	// }
	