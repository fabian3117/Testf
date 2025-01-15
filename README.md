# Testf
'''mermoid


graph TB
d098eb838e048773["```json
{
  "_id": "63d166c459f44903fbda9d20" ,
  "active_plan_id": "6724eea16b4ef0e633e3c7cf",
  "payment_ids": "F",
  "last_payment_id": "94538111700",
  "plan_corporativo": "67252ddd716e061daf9ee6b6" ,
  "nacimiento": "23/10/1996",
  "preferred_payment_method": "tarjeta",
  "status": "baja",
  "cobros_recurrentes": 3,
  "nombre": "Gian franco",
  "apellido": "Meloni",
  "email": "Gianfranqqo@gmail.com",
  "domicilio": "F",
  "celular": "1136245631",
  "documento": "39960260",
  "brand_name": "SportClub",
  "discounts": [],
  "cards": "F",
  "apto_medico": "F",
  "history": "F",
  "poi": "F",
  "next_payment_date": "2024-12-03T15:00:00.000+00:00",
  "fecha_vigencia": "2025-01-04T15:00:00.000Z",
  "last_subscription_date": "2024-11-04T13:43:47.362Z",
  "period_init_day": 4,
  "sportaccess_id": "MUVI-39960260",
  "mercadopago_id": "157802430-PBL7VtHbDYJ95a",
  "active_card": "9509814033",
  "token_status": "created",
  "token_spice": "tapBmSNkKJWX",
  "lastModified":  "2024-11-27T10:07:00.743Z",
  "version_control": "F",
  "documento_tipo": "dni",
  "genero": "Masculino",
  "seller_merchant_id": "6564b7a3481c8ecadde29720",





}
```"]
json-data["```json
{
  "_id": "63d166c459f44903fbda9d20" ,
  "active_plan_id": "6724eea16b4ef0e633e3c7cf",
  "payment_ids": "F",
  "last_payment_id": "94538111700",
  "plan_corporativo": "67252ddd716e061daf9ee6b6" ,
  "nacimiento": "23/10/1996",
  "preferred_payment_method": "tarjeta",
  "status": "baja",
  "cobros_recurrentes": 3,
  "nombre": "Gian franco",
  "apellido": "Meloni",
  "email": "Gianfranqqo@gmail.com",
  "domicilio": "F",
  "celular": "1136245631",
  "documento": "39960260",
  "brand_name": "SportClub",
  "discounts": [],
  "cards": "F",
  "apto_medico": "F",
  "history": "F",
  "poi": "F",
  "next_payment_date": "2024-12-03T15:00:00.000+00:00",
  "fecha_vigencia": "2025-01-04T15:00:00.000Z",
  "last_subscription_date": "2024-11-04T13:43:47.362Z",
  "period_init_day": 4,
  "sportaccess_id": "MUVI-39960260",
  "mercadopago_id": "157802430-PBL7VtHbDYJ95a",
  "active_card": "9509814033",
  "token_status": "created",
  "token_spice": "tapBmSNkKJWX",
  "lastModified":  "2024-11-27T10:07:00.743Z",
  "version_control": "F",
  "documento_tipo": "dni",
  "genero": "Masculino",
  "seller_merchant_id": "6564b7a3481c8ecadde29720" ,
"flex": {
    "gasto_mensual": 4000,
    "nivel_acceso_actual": "FLEX",
    "miembro_nuevo": true
  }
}
```"]
f99481c91eb70035["## Cliente normal"]
d1e94a1d75b88faa["## Cliente flex"]
4504b54b01b73407["### Objeto flex
#### Primer indicio de pertenecer a flex
#### Ver condiciones de creacion F1
"]
ecf5ba5232d28d83["```json
"flex": {
    "gasto_mensual": 4000,
    "nivel_acceso_actual": "FLEX",
    "miembro_nuevo": true
  }
```"]
afb5fdb33de694d4["```json
{
pending_flex_accesses: "4000"
}
```"]
3f87a899a11aa292["## Acumulativo de deuda
#### Ver condiciones de creacion F2
"]
16888b4a3ee27457["### Planes"]
fe933607bde4b526["```json 
{
  "_id": "6724ef3e4f22ce90ec06f221",
  "name": "Flex Anual Ecommerce",
  "slug": "Flex-Anual-Ecommerce",
  "price": 432000,
  "descripcion": "Flex Anual Ecommerce",
  "nivel_de_acceso": "Flex",
  "cobro": "Anual",
  "checkout": "https://pagar.sportclub.com.ar/paso2/Flex-Anual-Ecommerce",
  "cuotas": 1,
  "merchant_id":"6564b7a3481c8ecadde29720",
  "sede_local": null,
  "payment_methods": {
    "crypto": false,
    "efectivo": true,
    "tarjeta": true
  },
  "tyc": "F",
  "contacto": "elianamiranda@sportclub.team",
  "archivado": false,
  "deleted": false,
  "application_fee": 0,
  "created_by": "elianamiranda@sportclub.team",
  "created_at": "2024-11-01T15:09:50.658Z",
  "flex": {
    "costos_nivel_acceso": {
      "FLEX": {
        "costo_ingreso": 0,
        "tope_consumo": 24000
      },
      "PLUS": {
        "costo_ingreso": 2000,
        "tope_consumo": 24000
      },
      "TOTAL": {
        "costo_ingreso": 4000,
        "tope_consumo": 24000
      }
    },
    "nivel_acceso_maximo": "total"
  },
  "titulo-plan": "Flex Anual Ecommerce",
  "texto-condicion-plan": "Flex Anual Ecommerce",
  "descripcion-plan": "Flex Anual Ecommerce",
  "disclaimer": "",
  "prestaciones": "",
  "tipo-de-plan": "central",
  "version_control": "F"
}
```"]
cce11f4a81273f30["```mermaid
classDiagram

class flex{
+ CostosNivelAcceso : List<Costo>
+ nivel_acceso_maximo : String
}
class CostosNivelAcceso {
  + FLEX: Costo
  + PLUS: Costo
  + TOTAL: Costo
}

class Costo {
  + costo_ingreso: Integer
  + tope_consumo: Integer
}
flex --> CostosNivelAcceso
CostosNivelAcceso --> Costo
```"]
993f559d3f348e40["### Plan Flex
Es flex si contiene el objeto flex ( Esta vinculado al flex del cliente pero no es el mismo )"]
c8af8fcf7d18f887["```json
{
  "_id": "62cebcfad466496a4f582dce",
  "slug": "plan-plus-mensual-ecommerce",
  "price": 50000,
  "descripcion": "Incluye sedes categoría plus",
  "cobro": "Mensual",
  "checkout": "https://pagar.sportclub.com.ar/paso2/plan-plus-mensual-ecommerce",
  "texto-condicion-plan": "Mensual",
  "prestaciones": "<ul></ul>",
  "name": "Plan Plus Mensual Ecommerce",
  "merchant_id":"6564b7a3481c8ecadde29720",
  "sede_local": null,
  "payment_methods": {
    "crypto": false,
    "efectivo": true,
    "tarjeta": true
  },
  "contacto": "atencion.socios@sportclub.com.ar ",
  "archivado": false,
  "created_by": "agustina.jorda+superadmin@gmail.com",
  "created_at": "2022-07-13T12:39:22.633Z",
  "acepta-cuotas": false,
  "titulo-plan": "Plan Plus Mensual",
  "tyc": "F",
  "version_control": "f",
  "nivel_de_acceso": "Plus",
  "disclamer": "<p>* No incluye sedes Al Río, Ushuaia y mujer pilar</p>",
  "deleted": false,
  "descripcion-plan": "",
  "tipo-de-plan": "central",
  "application_fee": 0,
  "cuotas": 1
}"]
7d7a10599c2592f3["### Plan Normal"]
c079449da91c7bbf["```json
{
  "_id": "63d166c459f44903fbda9d20" ,
  "active_plan_id": "6724eea16b4ef0e633e3c7cf",
  "payment_ids": "F",
  "last_payment_id": "94538111700",
  "plan_corporativo": "67252ddd716e061daf9ee6b6" ,
  "nacimiento": "23/10/1996",
  "preferred_payment_method": "tarjeta",
  "status": "baja",
  "cobros_recurrentes": 3,
  "nombre": "Gian franco",
  "apellido": "Meloni",
  "email": "Gianfranqqo@gmail.com",
  "domicilio": "F",
  "celular": "1136245631",
  "documento": "39960260",
  "brand_name": "SportClub",
  "discounts": [],
  "cards": "F",
  "apto_medico": "F",
  "history": "F",
  "poi": "F",
  "next_payment_date": "2024-12-03T15:00:00.000+00:00",
  "fecha_vigencia": "2025-01-04T15:00:00.000Z",
  "last_subscription_date": "2024-11-04T13:43:47.362Z",
  "period_init_day": 4,
  "sportaccess_id": "MUVI-39960260",
  "mercadopago_id": "157802430-PBL7VtHbDYJ95a",
  "active_card": "9509814033",
  "token_status": "created",
  "token_spice": "tapBmSNkKJWX",
  "lastModified":  "2024-11-27T10:07:00.743Z",
  "version_control": "F",
  "documento_tipo": "dni",
  "genero": "Masculino",
  "seller_merchant_id": "6564b7a3481c8ecadde29720",





}
```"]
d579e67f58c6dad3["## Ciclo de vida
Cliente Flex"]
97ddae955b2a949e["```json
{
  "_id": "63d166c459f44903fbda9d20" ,
  "active_plan_id": "6724eea16b4ef0e633e3c7cf",
  "payment_ids": "F",
  "last_payment_id": "94538111700",
  "plan_corporativo": "67252ddd716e061daf9ee6b6" ,
  "nacimiento": "23/10/1996",
  "preferred_payment_method": "tarjeta",
  "status": "baja",
  "cobros_recurrentes": 3,
  "nombre": "Gian franco",
  "apellido": "Meloni",
  "email": "Gianfranqqo@gmail.com",
  "domicilio": "F",
  "celular": "1136245631",
  "documento": "39960260",
  "brand_name": "SportClub",
  "discounts": [],
  "cards": "F",
  "apto_medico": "F",
  "history": "F",
  "poi": "F",
  "next_payment_date": "2024-12-03T15:00:00.000+00:00",
  "fecha_vigencia": "2025-01-04T15:00:00.000Z",
  "last_subscription_date": "2024-11-04T13:43:47.362Z",
  "period_init_day": 4,
  "sportaccess_id": "MUVI-39960260",
  "mercadopago_id": "157802430-PBL7VtHbDYJ95a",
  "active_card": "9509814033",
  "token_status": "created",
  "token_spice": "tapBmSNkKJWX",
  "lastModified":  "2024-11-27T10:07:00.743Z",
  "version_control": "F",
  "documento_tipo": "dni",
  "genero": "Masculino",
  "seller_merchant_id": "6564b7a3481c8ecadde29720" ,
"flex": {
    "gasto_mensual": 0,
    "nivel_acceso_actual": "",
    "miembro_nuevo": true
  }
}
```"]
b68e6e5c11d7cb76["## Ingresa a sede
SEDE : TOTAL
GASTO ACCESO = 4000"]
990be40faffbc6d8["```json
{
  "_id": "63d166c459f44903fbda9d20" ,
  "active_plan_id": "6724eea16b4ef0e633e3c7cf",
  "payment_ids": "F",
  "last_payment_id": "94538111700",
  "plan_corporativo": "67252ddd716e061daf9ee6b6" ,
  "nacimiento": "23/10/1996",
  "preferred_payment_method": "tarjeta",
  "status": "baja",
  "cobros_recurrentes": 3,
  "nombre": "Gian franco",
  "apellido": "Meloni",
  "email": "Gianfranqqo@gmail.com",
  "domicilio": "F",
  "celular": "1136245631",
  "documento": "39960260",
  "brand_name": "SportClub",
  "discounts": [],
  "cards": "F",
  "apto_medico": "F",
  "history": "F",
  "poi": "F",
  "next_payment_date": "2024-12-03T15:00:00.000+00:00",
  "fecha_vigencia": "2025-01-04T15:00:00.000Z",
  "last_subscription_date": "2024-11-04T13:43:47.362Z",
  "period_init_day": 4,
  "sportaccess_id": "MUVI-39960260",
  "mercadopago_id": "157802430-PBL7VtHbDYJ95a",
  "active_card": "9509814033",
  "token_status": "created",
  "token_spice": "tapBmSNkKJWX",
  "lastModified":  "2024-11-27T10:07:00.743Z",
  "version_control": "F",
  "documento_tipo": "dni",
  "genero": "Masculino",
  "seller_merchant_id": "6564b7a3481c8ecadde29720" ,
"flex": {
    "gasto_mensual": 4000,
    "nivel_acceso_actual": "TOTAL",
    "miembro_nuevo": true
  }
}
```"]
5e4049a1ea79e495["### Se da de baja"]
643666d173e1f9c1["```json
{
  "_id": "63d166c459f44903fbda9d20" ,
  "active_plan_id": "6724eea16b4ef0e633e3c7cf",
  "payment_ids": "F",
  "last_payment_id": "94538111700",
  "plan_corporativo": "67252ddd716e061daf9ee6b6" ,
  "nacimiento": "23/10/1996",
  "preferred_payment_method": "tarjeta",
  "status": "baja",
  "cobros_recurrentes": 3,
  "nombre": "Gian franco",
  "apellido": "Meloni",
  "email": "Gianfranqqo@gmail.com",
  "domicilio": "F",
  "celular": "1136245631",
  "documento": "39960260",
  "brand_name": "SportClub",
  "discounts": [],
  "cards": "F",
  "apto_medico": "F",
  "history": "F",
  "poi": "F",
  "next_payment_date": "2024-12-03T15:00:00.000+00:00",
  "fecha_vigencia": "2025-01-04T15:00:00.000Z",
  "last_subscription_date": "2024-11-04T13:43:47.362Z",
  "period_init_day": 4,
  "sportaccess_id": "MUVI-39960260",
  "mercadopago_id": "157802430-PBL7VtHbDYJ95a",
  "active_card": "9509814033",
  "token_status": "created",
  "token_spice": "tapBmSNkKJWX",
  "lastModified":  "2024-11-27T10:07:00.743Z",
  "version_control": "F",
  "documento_tipo": "dni",
  "genero": "Masculino",
  "seller_merchant_id": "6564b7a3481c8ecadde29720" ,
  "pending_flex_accesses" : "4000",
	"flex": {
	    "gasto_mensual": 0,
	    "nivel_acceso_actual": "",
	    "miembro_nuevo": true
  }
}
```"]
46c6c82fe9344f26["```json
{
  "_id": "63d166c459f44903fbda9d20" ,
  "active_plan_id": "6724eea16b4ef0e633e3c7cf",
  "payment_ids": "F",
  "last_payment_id": "94538111700",
  "plan_corporativo": "67252ddd716e061daf9ee6b6" ,
  "nacimiento": "23/10/1996",
  "preferred_payment_method": "tarjeta",
  "status": "baja",
  "cobros_recurrentes": 3,
  "nombre": "Gian franco",
  "apellido": "Meloni",
  "email": "Gianfranqqo@gmail.com",
  "domicilio": "F",
  "celular": "1136245631",
  "documento": "39960260",
  "brand_name": "SportClub",
  "discounts": [],
  "cards": "F",
  "apto_medico": "F",
  "history": "F",
  "poi": "F",
  "next_payment_date": "2024-12-03T15:00:00.000+00:00",
  "fecha_vigencia": "2025-01-04T15:00:00.000Z",
  "last_subscription_date": "2024-11-04T13:43:47.362Z",
  "period_init_day": 4,
  "sportaccess_id": "MUVI-39960260",
  "mercadopago_id": "157802430-PBL7VtHbDYJ95a",
  "active_card": "9509814033",
  "token_status": "created",
  "token_spice": "tapBmSNkKJWX",
  "lastModified":  "2024-11-27T10:07:00.743Z",
  "version_control": "F",
  "documento_tipo": "dni",
  "genero": "Masculino",
  "seller_merchant_id": "6564b7a3481c8ecadde29720" ,
  "pending_flex_accesses":4000
}
```"]
2535db8789399719["### Se pasa a plan normal
"]
37349c7f0471bdb3["El objeto flex se elimina 
Pero queda la referencia a la deuda como el ==pending_flex_accesses=="]
2a2d21d180dcac79["#### Si se cambia entre flex - normal
Alterna correctamente entre estas versiones manteniendo la consistencia"]
json-data --> 4504b54b01b73407
4504b54b01b73407 --> ecf5ba5232d28d83
3f87a899a11aa292 --> afb5fdb33de694d4
fe933607bde4b526 --> cce11f4a81273f30
97ddae955b2a949e --> b68e6e5c11d7cb76
b68e6e5c11d7cb76 --> 990be40faffbc6d8
990be40faffbc6d8 --> |Puede repetirse 
ciclicamente 

Hasta finalizar periodo| b68e6e5c11d7cb76
990be40faffbc6d8 --> 5e4049a1ea79e495
5e4049a1ea79e495 --> 643666d173e1f9c1
990be40faffbc6d8 --> 2535db8789399719
37349c7f0471bdb3 --> 46c6c82fe9344f26
990be40faffbc6d8 --> 2a2d21d180dcac79
46c6c82fe9344f26 --> 2a2d21d180dcac79
2a2d21d180dcac79 --> 990be40faffbc6d8
2a2d21d180dcac79 --> 46c6c82fe9344f26
style json-data fill:#FFD700, stroke:#cca400
style 97ddae955b2a949e fill:#FFD700, stroke:#cca400
style 990be40faffbc6d8 fill:#FFD700, stroke:#cca400
style 643666d173e1f9c1 fill:#FFD700, stroke:#cca400
style 46c6c82fe9344f26 fill:#FFD700, stroke:#cca400


'''
