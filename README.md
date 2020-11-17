# Desafio Venda.la

O desafio é fazer um programa que converta o código ZPL para HTML.

## O que você precisa fazer

Você precisa criar uma API utilizando qualquer linguagem de programação que vai receber um ZPL e transformar em HTML

## Seria legal ...

- Rodar na Nuvem

## Exemplos de ZPls

Exemplo 1
```
^XA
^CI28
^FX Logo Meli^FS
^FO20,10^GFA,800,800,10,,:::::::::::O0FF,M07JFE,L07FC003FE,K07EL07E,J01EN078,J07P0E,I01CP038,I07R0E,001CK01FK038,003L0IFK0C,0078J03803CJ0E,0187J06I07I01D8,0300F00F8J0FEFE0C,02003IFK01J06,04I01C6P02,08K0401FM01,1L08060CM083K0100C02M0C2M01001M046K0306I0CL064K0198I02L024Q01L02CR08K03CR04K03FR02K03FFQ01J07!C1FQ0C007E3C03EP0203F03C0078O010F003CI0EF1N0F8003CI070C4M06I03CI02003CL02I03CI02P02I036I03N0106I066I01J08J0C4I067J0EI08J078I0E38I03I0E00406I01C3CI01800100204I01C3CJ0FI080118I03C1EJ03800801FJ0780FK0C008018J0F,078J07C0823J01F,07EJ01C1C36J07E,03FK031C3K0FC,01FCJ01E18J01F8,00FER07F,007F8P01FE,003FFP0FFC,I0FFEN07FF,I03FFCL03FFC,J0IFCJ03IF,J07PFE,K0PF,K01NF8,L01LF8,N0JF,,:::::::::::^FS
^FO120,22^A0N,24,24^FDDaniela Brito da Silva #377903096^FS
^FO120,45^A0N,24,24^TBN,660,54^FDRua Doutor Antônio Bento 560
, Santo Amaro^FS
^FO120,92^A0N,24,24^TBN,660,54^FD
São Paulo
, SP
 - CEP 04750001^FS
^FO120,135^A0N,24,24^FDVenda: 41643^FS
^FO255,132^A0N,27,27^FD32208^FS
^FO550,135^A0N,24,24^FDEnvio: 4022272^FS
^FO702,132^A0N,27,27^FD0232^FS
^FX 1 Horizontal Line ^FS
^FO0,170^GB850,0,2^FS
^FO0,185^A0N,48,48^FB800,1,0,C^FDMercado Envios Flex^FS
^FX 2 Horizontal Line ^FS
^FO0,235^GB850,0,2^FS
^FX QR Code ^FS
^FO260,270^BY4,4,0^BQN,2,7^FDLA,{"id":"40222720232","sender_id":377903096,"hash_code":"u3g+R04HlioVY2GpAQkzZ+vW/MZJqf74vx5P99Edeas=","security_digit":"0"}^FS
^FO0,585^A0N,48,48^FB800,1,0,C^FD Sao Bernardo 1^FS
^FO0,640^A0N,45,45^FB800,1,0,C^FDAssunção^FS
^FX 3 Horizontal Line ^FS
^FO0,700^GB850,0,2^FS
^FO40,720^A0N,28,28^TBN,730,56^FDDestinatario: Kelly Cutti^FS
^FO39,720^A0N,28,28^FDDestinatario:^FS
^FO40,719^A0N,28,28^FDDestinatario:^FS
^FO40,790^A0N,28,28^FDNickname: KELLYCUTTI^FS
^FX 4 Horizontal Line ^FS
^FO0,850^GB820,0,2 ^FS
^FO40,880^A0N,28,28^TBN,730,56^FDEndereço: Avenida José Odorizzi 2249^FS
^FO39,880^A0N,28,28^FDEndereço:^FS
^FO40,879^A0N,28,28^FDEndereço:^FS
^FO40,960^A0N,28,28^TBN,730,94^FDComplemento: Bl 04 Apto34^FS
^FO39,960^A0N,28,28^FDComplemento:^FS
^FO40,959^A0N,28,28^FDComplemento:^FS
^FO40,1080^A0N,28,28^TBN,730,56^FDCidade: São Bernardo do Campo
, SP^FS
^FO39,1080^A0N,28,28^FDCidade:^FS
^FO40,1079^A0N,28,28^FDCidade:^FS
^FO40,1120^A0N,28,28^TBN,730,56^FDCEP: 09861001^FS
^FO39,1120^A0N,28,28^FDCEP:^FS
^FO40,1119^A0N,28,28^FDCEP:^FS
^FO765,850^GB0,350,45^FS
^FO770,900^A0B,26,26^FR^FDEndereço residencial^FS
^XZ
```

Exemplo 2
```
^XA
^CI28
^LH0,0
^FX  HEADER  ^FS
^FX Logo_Meli ^FS
^FO20,10^GFA,800,800,10,,:::::::::::O0FF,M07JFE,L07FC003FE,K07EL07E,J01EN078,J07P0E,I01CP038,I07R0E,001CK01FK038,003L0IFK0C,0078J03803CJ0E,0187J06I07I01D8,0300F00F8J0FEFE0C,02003IFK01J06,04I01C6P02,08K0401FM01,1L08060CM083K0100C02M0C2M01001M046K0306I0CL064K0198I02L024Q01L02CR08K03CR04K03FR02K03FFQ01J07!C1FQ0C007E3C03EP0203F03C0078O010F003CI0EF1N0F8003CI070C4M06I03CI02003CL02I03CI02P02I036I03N0106I066I01J08J0C4I067J0EI08J078I0E38I03I0E00406I01C3CI01800100204I01C3CJ0FI080118I03C1EJ03800801FJ0780FK0C008018J0F,078J07C0823J01F,07EJ01C1C36J07E,03FK031C3K0FC,01FCJ01E18J01F8,00FER07F,007F8P01FE,003FFP0FFC,I0FFEN07FF,I03FFCL03FFC,J0IFCJ03IF,J07PFE,K0PF,K01NF8,L01LF8,N0JF,,:::::::::::^FS
^FO130,20^A0N,24,24^FDDaniela Brito da Silva #377903096^FS
^FO130,43^A0N,24,24^TBN,530,54^FDEstrada Particular Sadae Takagi 2235, Cooperativa^FS
^FO130,90^A0N,24,24^TBN,530,54^FDSão Bernardo do Campo, BR-SP - 09852070^FS
^FO130,120^A0N,24,24^FDVenda: 41645^FS
^FO265,117^A0N,27,27^FD13448^FS
^FO400,120^A0N,24,24^FDSKU: MC022KABABY^FS
^FO480,150^GB330,40,40^FS
^FO410,160^A0N,22,22
^FB460,1,0,C^FR^FDENTREGAR NA COLETA^FS
^FX  Shipment_Number_Bar_Code  ^FS
^FO160,210^BY3,,0^BCN,160,N,N,N^FD>:40222882887^FS
^FO0,385^A0N,30,30^FB404,1,0,R^FD4022288^FS
^FO405,380^A0N,35,35^FB404,1,0,L^FD2887^FS
^FX  END_HEADER  ^FS
^FO20,420^GB240,60,3^FS
^FO20,433^A0N,40,34
^FB240,1,0,C^FDXSP4 | 04:00
^FS
^FO20,480^GB240,57,57^FS
^FO20,485^A0N,50,50
^FB240,1,0,C^FR^FDSSC2^FS
^FO280,420^GB240,60,3^FS
^FO280,433^A0N,40,34
^FB240,1,0,C^FDSSC2^FS
^FO280,480^GB240,57,57^FS
^FO280,485^A0N,50,50
^FB240,1,0,C^FR^FD3_10^FS
^FX  IN/OUT Route Box  ^FS
^FX  FIRST CLUSTER  ^FS
^FO20,150^GB420,45,3^FS
^FO20,156^A0N,45,45
^FB210,1,0,C^FR^FDXSP4^FS
^FX  LAST CLUSTER  ^FS
^FO229,153^GB210,40,40^FS
^FO229,156^A0N,45,45
^FB210,1,0,C^FR^FDSSC2^FS
^FX  CUSTOM_DATA  ^FS
^FO15,710^A0N,105,105^FB410,1,0,C^FDSSC2^FS
^FO410,710^A0N,105,105^FB410,1,0,C^FD3_10^FS
^FO0,840^A0N,40,40^FB820,1,0,C^FDQUI 19/11/2020^FS
^FO0,890^A0N,40,40^FB820,1,0,C^FDCEP: 88048417^FS^FX  END CUSTOM_DATA  ^FS
^FO0,950^GB850,0,2^FS
^FX  RECEIVER ZONE  ^FS
^FO30,970^A0N,26,26^FB600,2,0,L^FDJosmara Echeverria (ECJA1475370)^FS
^FO30,1030^A0N,26,26^FB600,2,0,L^FDEndereço: Servidão Sotero José de Farias 554, Rio Tavares - Campeche^FS
^FO30,1090^A0N,30,30^FDCEP: 88048417^FS
^FO30,1089^A0N,30,30^FDCEP: 88048417^FS
^FO230,1090^A0N,30,30^FDTelefone: 45998092316^FS
^FO230,1089^A0N,30,30^FDTelefone: 45998092316^FS
^FO30,1121^A0N,26,26^FB600,2,1000,L^FDCidade de destino: Florianópolis, Santa Catarina^FS
^FO30,1150^A0N,26,26^FB600,5,0,L^FDComplemento: ^FS
^FX  QR Code  ^FS
^FO650,985^BY2,2,0^BQN,2,5^FDLA,{"id":"40222882887"}^FS
^FO650,1130^GB105,40,40^FS
^FO650,1135^A0N,35,35
^FB105,1,0,C^FR^FDR^FS
^FX  END_FOOTER  ^FS
^XZ

```

Exemplo 3
```
^XA
^CI28
^LH0,0
^FX  HEADER  ^FS
^FX Logo_Meli ^FS
^FO20,10^GFA,800,800,10,,:::::::::::O0FF,M07JFE,L07FC003FE,K07EL07E,J01EN078,J07P0E,I01CP038,I07R0E,001CK01FK038,003L0IFK0C,0078J03803CJ0E,0187J06I07I01D8,0300F00F8J0FEFE0C,02003IFK01J06,04I01C6P02,08K0401FM01,1L08060CM083K0100C02M0C2M01001M046K0306I0CL064K0198I02L024Q01L02CR08K03CR04K03FR02K03FFQ01J07!C1FQ0C007E3C03EP0203F03C0078O010F003CI0EF1N0F8003CI070C4M06I03CI02003CL02I03CI02P02I036I03N0106I066I01J08J0C4I067J0EI08J078I0E38I03I0E00406I01C3CI01800100204I01C3CJ0FI080118I03C1EJ03800801FJ0780FK0C008018J0F,078J07C0823J01F,07EJ01C1C36J07E,03FK031C3K0FC,01FCJ01E18J01F8,00FER07F,007F8P01FE,003FFP0FFC,I0FFEN07FF,I03FFCL03FFC,J0IFCJ03IF,J07PFE,K0PF,K01NF8,L01LF8,N0JF,,:::::::::::^FS
^FO130,20^A0N,24,24^FDDaniela Brito da Silva #377903096^FS
^FO130,43^A0N,24,24^TBN,530,54^FDEstrada Particular Sadae Takagi 2235, Cooperativa^FS
^FO130,90^A0N,24,24^TBN,530,54^FDSão Bernardo do Campo, BR-SP - 09852070^FS
^FO130,120^A0N,24,24^FDVenda: 41648^FS
^FO265,117^A0N,27,27^FD67181^FS
^FO400,120^A0N,24,24^FDSKU: MC003KITCLINK^FS
^FO480,150^GB330,40,40^FS
^FO410,160^A0N,22,22
^FB460,1,0,C^FR^FDENTREGAR NA COLETA^FS
^FX  Shipment_Number_Bar_Code  ^FS
^FO160,210^BY3,,0^BCN,160,N,N,N^FD>:40223192457^FS
^FO0,385^A0N,30,30^FB404,1,0,R^FD4022319^FS
^FO405,380^A0N,35,35^FB404,1,0,L^FD2457^FS
^FX  END_HEADER  ^FS
^FO20,420^GB240,60,3^FS
^FO20,433^A0N,40,34
^FB240,1,0,C^FDXSP4 | 03:00
^FS
^FO20,480^GB240,57,57^FS
^FO20,485^A0N,50,50
^FB240,1,0,C^FR^FDSSP5^FS
^FO280,420^GB240,60,3^FS
^FO280,433^A0N,40,34
^FB240,1,0,C^FDSSP5^FS
^FO280,480^GB240,57,57^FS
^FO280,485^A0N,50,50
^FB240,1,0,C^FR^FDA7_5^FS
^FX  IN/OUT Route Box  ^FS
^FX  FIRST CLUSTER  ^FS
^FO20,150^GB420,45,3^FS
^FO20,156^A0N,45,45
^FB210,1,0,C^FR^FDXSP4^FS
^FX  LAST CLUSTER  ^FS
^FO229,153^GB210,40,40^FS
^FO229,156^A0N,45,45
^FB210,1,0,C^FR^FDSSP5^FS
^FX  CUSTOM_DATA  ^FS
^FO15,710^A0N,105,105^FB410,1,0,C^FDSSP5^FS
^FO410,710^A0N,105,105^FB410,1,0,C^FDA7_5^FS
^FO0,840^A0N,40,40^FB820,1,0,C^FDQUA 18/11/2020^FS
^FO0,890^A0N,40,40^FB820,1,0,C^FDCEP: 06700229^FS^FX  END CUSTOM_DATA  ^FS
^FO0,950^GB850,0,2^FS
^FX  RECEIVER ZONE  ^FS
^FO30,970^A0N,26,26^FB600,2,0,L^FDTatiane Barboza (ROBERTOFRANCISCOWILSON)^FS
^FO30,1030^A0N,26,26^FB600,2,0,L^FDEndereço: Rua Metal Leve 181, Jardim Leonor^FS
^FO30,1090^A0N,30,30^FDCEP: 06700229^FS
^FO30,1089^A0N,30,30^FDCEP: 06700229^FS
^FO230,1090^A0N,30,30^FDTelefone: 11932773578^FS
^FO230,1089^A0N,30,30^FDTelefone: 11932773578^FS
^FO30,1121^A0N,26,26^FB600,2,1000,L^FDCidade de destino: Cotia, São Paulo^FS
^FO30,1150^A0N,26,26^FB600,5,0,L^FDComplemento: ^FS
^FX  QR Code  ^FS
^FO650,985^BY2,2,0^BQN,2,5^FDLA,{"id":"40223192457"}^FS
^FO650,1130^GB105,40,40^FS
^FO650,1135^A0N,35,35
^FB105,1,0,C^FR^FDR^FS
^FX  END_FOOTER  ^FS
^XZ
```

## Premiação

Após homologado e testado em nossos servidores será pago R$ 1.000,00

Se você tiver alguma dúvida, entrar em contato com graziani@vendala.com.br.

Ao finalizar o teste, subir em um reposítorio público, mandar o link para graziani@vendala.com.br

---

Boa sorte!
