# Config perso live template #

----------
## Mise à jour ##

Se placer dans C:\Users\name\\.WebIde80\config\templates. <br>

## Html zone ##

#### <? php if (): ?> ####

**`pif`**

	<?php if($COND$): ?>
    $END$
	<?php endif; ?>

#### <?php elseif(): ?> ####

**`pelseif`**

	<?php elseif($COND$): ?>
	$END$

#### <?php else: ?> ####

**`pelse`**

    <?php else: ?>
	$END$	

## Php zone ##

#### var_dump(); die; ####

**`dd`**

	var_dump($var$);die;

#### header('Location: ') ####

**`loc`**

	header('Location: $VAR$');$END$

#### $bdd = new  PDO(' ... ') ####

**`bdd`**

	try{
	    $bdd = new PDO('mysql:host=$HOST$;dbname=$DBNAME$','$ACCESS$','$MDP$');
	} catch (Exception $e){
	    die('Erreur :'. $e->getMessage());
	}$END$

#### if ( ... ){ ... } ####

**`if`**

	if ($COND$){
	    $END$
	}

#### elseif ( ... ){ ... } ####

**`elseif`**

	elseif ($COND$){
	    $END$
	}

#### else{ ... } ####

**`else`**

	else{
	    $END$
	}

#### while ( ... ){ ... } ####

**`while`**

	while($COND$){
		$END$
	}

#### for ( $i = ; $i<= ; $i++ ){ ... } ####

**`for`**

	for ($i = $NUMBER$; $i <= $VAR$; $i++) {
	    $END$
	}


#### switch ( ... ){ ... } ####

**`switch`**

	switch ($VAR$){
	    case $VALUE$:
	        $EFFECT$;
	        break;
	    default:
	        $EFFECT2$;    
	}$END$