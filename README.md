Mercado Energético

Para incorporar la negociación de energía generada a partir de fuentes renovables específicas como paneles solares y energía eólica en el contrato inteligente en la blockchain de NEAR, podemos  añadir detalles adicionales a la oferta de energía. Esto permitirá a los vendedores especificar el tipo de fuente de energía de cada oferta y a los compradores seleccionar ofertas basadas en sus preferencias o necesidades de sostenibilidad.

Explicación del código:

Definición de Estructuras (EnergyOffer y EnergyContract):
EnergyOffer: Representa una oferta de venta de energía con detalles como ID del vendedor, cantidad de energía y precio por kWh.
EnergyContract: Define un contrato entre un comprador y un vendedor, especificando los detalles del acuerdo.
Mapas Persistentes:
Se usan para almacenar las ofertas y los contratos de forma segura y persistente en el estado del blockchain.


Funciones del Contrato:

registerOffer: Permite a un vendedor registrar una oferta de energía.
acceptOffer: Permite a un comprador aceptar una oferta, creando un contrato y asegurando el pago.
getOffers: Devuelve una lista de todas las ofertas activas.
getContracts: Proporciona una lista de todos los contratos energéticos existentes.
Enumeración RenewableType:
Define los tipos de energía renovable disponibles, en este caso solar y eólica.
EnergyOffer y EnergyContract:
energyType sirve para especificar el tipo de fuente de energía renovable de cada oferta y contrato. Esto ayuda a los participantes del mercado a tomar decisiones basadas en preferencias ecológicas o de sostenibilidad.
Registro y Aceptación de Ofertas:

Las funciones registerOffer y acceptOffer ahora manejan el tipo de energía, permitiendo a los usuarios negociar específicamente energía solar o eólica.

