# Access Control Manager

در هر سیستم access control manager یکی از مهمترین اجزای آن سیستم محسوب میشود  و با توجه به گستردگی اکوسیستم لایولی، ما تصمیم گرفتیم که یک access control manager را از صفر  طراحی کنیم که بتواند نیاز های لایولی رو برطرف نماید.

ایده اصلی این طراحی بر مبنای  یک ساختار access control manager متمرکز بر روی بستر blockchain  که یک ساختار غیرمتمرکز و on-chain هست ، ایجاد شده است

بر همین اساس و مطابق با شکل زیر ما نیاز به تعاریف مفاهیم در نظر گرفته شده در طراحی رو داریم

&#x20;

<figure><img src="../.gitbook/assets/lively-token-Page-3.drawio.svg" alt=""><figcaption></figcaption></figure>

Access Control Manager (ACM): it's main contract to access control in Lively system. it contains so many functions related to manage user, roles, groups, contexts and realms.&#x20;

Function: it's basic element in ACM that contains a function selector and only one role along with status which are assigned to it.&#x20;

Context: it contains a set of Functions with a unique id in ACM. In the registration process, the keccak256 of the contract address is used as a context id. actually, each Context is equivalent to each contract in ACM env. According to figure-2, when a contract registers itself in ACM, it creates registerContextRequest that contains an array of function selectors along with related roles then registerContext() of ACM is called by contract. if registration is completed successfully then the context Id is returned. eventually, when one of the contract functions is called then it calls hasAccess function of ACM to check user permission to call it.&#x20;

Realm: it defines a domain for set of Contexts with specific propose. each Realm doesn't any limitation to contain Context. ACM can contain unlimited Realm.

User: it's an entity that could be one of EOA or smart contracts.

Role: it contains set of users with clear definition of activity in Lively system that define in ACM.it can use in many Functions. &#x20;

Group: It contains set of Roles to facilitate policy management. ACM can contain unlimited Groups.

<figure><img src="../.gitbook/assets/lively-token-Page-10.drawio.svg" alt=""><figcaption></figcaption></figure>

ACM contract implements interfaces that relate to defined keywords. the UML diagram describe interfaces.

<figure><img src="../.gitbook/assets/lively-token-Page-2.drawio.svg" alt=""><figcaption></figcaption></figure>
