# Config perso live template #

----------

## Html zone ##
>pif

	<?php if($COND$): ?>
    $END$
	<?php endif; ?>

> pelsif

	<?php elseif($COND$): ?>
	$END$

> pelse

    <?php else: ?>
	$END$	

## Php zone ##

>dd

	var_dump($var$);die;

>loc 

	header('Location: $VAR$');$END$