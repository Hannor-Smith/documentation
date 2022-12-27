---
தலைப்பு: மேன் பக்கம் almost - வெண்ணிலா OS
விளக்கம்: almost பயன்பாட்டுக்கான மேன் பக்கம்.
---

# மேன் பக்கம் `almost`

## பெயர்

```
almost - (i)மாற்றக்கூடிய கோப்பு பண்புக்கூறு மற்றும் tmpfs ஆகியவற்றின் அடிப்படையில் தேவைக்கேற்ப மாறாத தன்மை மற்றும் அடுக்குதல் கருவி.
```

## SYNOPSIS

```
almost [விருப்பங்கள்] [கட்டளை] [ARGS]
```

## DESCRIPTION

```
almost - கணினி ரூட்டில் உள்ள கோப்புகள் மற்றும் கோப்பகங்களின் மாறாத தன்மையை மாற்றுவதன் மூலம் தேவைக்கேற்ப மாறாத தன்மையை வழங்கும் ஒரு பயன்பாடு. இது மாறாத கோப்பகங்களின் மேல் அடுக்குகளை உருவாக்குவதற்கான வழியையும் வழங்குகிறது, மாற்றங்களைச் செய்வதற்கு முன் அவற்றைச் சோதிக்க உங்களை அனுமதிக்கிறது.

விருப்பங்கள்:
	--help/-h		இந்த செய்தியை காட்டு
	--verbose/-v		verbose வெளியீடு
	--version/-V		பதிப்பைக் காட்டு

கட்டளைகள்:
	enter			மறுதொடக்கம் செய்யும் வரை கோப்பு முறைமையை ro அல்லது rw ஆக அமைக்கவும்
	config			தற்போதைய கட்டமைப்பைக் காட்டு
	check			கோப்பு முறைமை படிக்க மட்டுமே உள்ளதா அல்லது படிக்க-எழுதுகிறதா என்பதைச் சரிபார்க்கவும்
	run			ரீட்-ரைட் பயன்முறையில் ஒரு கட்டளையை இயக்குகிறது மற்றும் கட்டளை வெளியேறிய பிறகு படிக்க-மட்டும் பயன்முறைக்குத் திரும்புகிறது
```

## ENTER

```
மறுதொடக்கம் செய்யும் வரை கோப்பு முறைமையை படிக்க-மட்டும் அல்லது படிக்க-எழுதுமாறு அமைக்கவும்.

கோப்பு முறைமையை ரீட்-ரைட் பயன்முறையில் அமைப்பது ஒரு பாதுகாப்பு அபாயமாக இருக்கலாம்
இந்த கட்டளையைப் பயன்படுத்தும் போது கவனமாக இருங்கள்.

பயன்பாடு:
    enter [விருப்பங்கள்] [கட்டளை]

விருப்பங்கள்:
	--help/-h		இந்த செய்தியை காட்டு
	--verbose/-v		verbose வெளியீடு

விருப்பங்கள்:
	ro			கோப்பு முறைமையை படிக்க-மட்டும் அமைக்கவும்
	rw			கோப்பு முறைமையை படிக்க-எழுதுவதாக அமைக்கவும்
	default			உள்ளமைவு கோப்பில் வரையறுக்கப்பட்டுள்ளபடி கோப்பு முறைமையை அமைக்கவும்

எடுத்துக்காட்டுகள்:
	almost enter ro
	almost enter rw
```

## CONFIG (உள்ளமைவு)

```
தற்போதைய உள்ளமைவை நிர்வகித்து காண்பிக்கவும்.

பயன்பாடு:
    config [விருப்பங்கள்] [கட்டளை]

விருப்பங்கள்:
    --help/-h		இந்த செய்தியை காட்டு

விருப்பங்கள்:
    set [முக்கிய] [மதிப்பு]	ஒரு கட்டமைப்பு மதிப்பை அமைக்கவும்

எடுத்துக்காட்டுகள்:
    almost config
    almost config set Almost::DefaultMode 1
```

## CHECK (சரிபார்)

```
கோப்பு முறைமை படிக்க மட்டுமே உள்ளதா அல்லது படிக்க-எழுதுகிறதா என்பதைச் சரிபார்க்கவும்.

பயன்பாடு:
check [விருப்பங்கள்] [கட்டளை]
விருப்பங்கள்:
	--help/-h		இந்த செய்தியை காட்டு
எடுத்துக்காட்டுகள்:
	almost check
```

## RUN (ஓடு)

```
ரீட்-ரைட் பயன்முறையில் கட்டளையை இயக்குகிறது மற்றும் கட்டளை வெளியேறிய பிறகு படிக்க மட்டும் பயன்முறைக்கு திரும்பும்.

பயன்பாடு:
    run [கட்டளை]
விருப்பங்கள்:
	--help/-h		இந்த செய்தியை காட்டு
	--verbose/-v		verbose வெளியீடு
எடுத்துக்காட்டுகள்:
    almost run ls
```

## மேலும் பார்க்கவும்

- [`apx`](/docs/apx)

##  DIAGNOSTICS (பரிசோதனைகள்)

```
almost வெற்றியில் 0, பிழையில் 1 ஐ வழங்குகிறது.
```

## நூலாசிரியர்

```
வெண்ணிலா OS இன் பங்களிப்பாளர்கள்
```

## பிழைகளைப் புகாரளிப்பது 

[சிக்கல் டிராக்கருக்கு] (https://github.com/Vanilla-OS/almost/issues) பிழைகளைப் புகாரளிக்கவும்.