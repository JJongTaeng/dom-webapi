# dom-webapi

# 함수형 프로그래밍과 ES6+ 예제 코드

## 목차

1. [DOM 기본 개념](#dom-기본-개념)
2. [Document 인터페이스](#document-인터페이스)
3. [Element 인터페이스](#element-인터페이스)
4. [Element 인터페이스: NamedNodeMap](#element-인터페이스-namednodemap)
5. [Element 인터페이스: 속성 메소드](#element-인터페이스-속성-메소드)
6. [namespace를 사용한 속성 처리](#namespace를-사용한-속성-처리)
7. [DOMImplementation 인터페이스](#domimplementation-인터페이스)
8. [Node 인터페이스](#node-인터페이스)
9. [Node Tree Position 프로퍼티](#node-tree-position-프로퍼티)
10. [Node Tree 포지션 비교](#node-tree-포지션-비교)
11. [Node 추가, 삭제, 대체, 복제](#node-추가-삭제-대체-복제)
12. [DOM Traversal](#dom-traversal)
13. [DocumentFragment 인터페이스](#documentfragment-인터페이스)
14. [텍스트 처리 인터페이스](#텍스트-처리-인터페이스)
15. [HTML 스펙의 Document 인터페이스](#html-스펙의-document-인터페이스)
16. [Window 인터페이스](#window-인터페이스)
17. [Navigator 인터페이스](#navigator-인터페이스)
18. [Messaging System](#messaging-system)
19. [WindowOrWorkerGlobalScope 인터페이스](#windoworworkerglobalscope-인터페이스)



## DOM 기본 개념

### 자바스크립트 대응 용어 정리: HTML과 자바스크립트, CSS와 자바스크립트
### DOM Document, HTML Document 인터페이스
### 노드(Node): HTML과 DOM 트리, 노드 타입
### Node Tree: 노드 위치 표현, 트리(Tree), Tree Order, 노드 트리, 구조/위치
### DOM 랜더링 차이: 노드 트리 차이, 텍스트 노드 제외, 노드 트리/인터페이스
**[⬆ 상단으로](#목차)**


## Document 인터페이스

### Document 프로퍼티: DocumentType, doctype 형태, document 프로퍼티
### 엘리먼트 추출-1: getElementById(), getElementsByClassName()
### HTMLCollection 인터페이스: HTMLCollection, item(), namedItem()
### NodeList 인터페이스: NodeList, item()
### childNodes, children 프로퍼티 차이 
### Event 개념: Event 요소
### 이벤트 설정 형태: 이벤트 리스너와 핸들러
### live, static
### 엘리먼트 추출-2: getElementsByTagName(), getElementsByTagNameNS()
### 엘리먼트 오브젝트 생성: createElement(), createElementNS()
**[⬆ 상단으로](#목차)**


## Element 인터페이스

### XML 형태
### XML과 Namespace
### content 속성, IDL 속성
### 자바스크립트로 속성값을 구하는 형태
### DOMTokenList 인터페이스-1
### DOMTokenList 인터페이스-2
### DOMTokenList 인터페이스-3
**[⬆ 상단으로](#목차)**


## Element 인터페이스: NamedNodeMap

### NamedNodeMap 인터페이스-1
### NamedNodeMap 인터페이스-2
### NamedNodeMap 인터페이스-3
**[⬆ 상단으로](#목차)**


## Element 인터페이스: 속성 메소드

### 속성 작성 여부: hasAttribute(), hasAttributes()
### 속성 작성 체크: hasAttribute(), hasAttributes()
### 속성값 추출: getAttribute() 
### 속성 추출: 이름, 노드, getAttributeNames(), getAttributeNode()
### 속성 생성: Attr 오브젝트, createAttribute()
### 속성 생성: namespace 사용, createAttributeNS()
### Attr 인터페이스
### 속성 설정-1: setAttribute()
### 속성 설정-2: setAttribute(), setAttributeNode()
### 속성 삭제: removeAttribute(), removeAttributeNode()
### 속성 토글: toggleAttribute(), toggle 활용 맛보기
**[⬆ 상단으로](#목차)**


## namespace를 사용한 속성 처리

### 속성 존재 여부, 속성값 추출: hasAttributeNS(), getAttributeNS()
### 속성 설정, 속성 삭제: setAttributeNS(), removeAttributeNS()
**[⬆ 상단으로](#목차)**


## DOMImplementation 인터페이스

### DOMImplementation 인터페이스-1: implementation, createHTMLDocument()
### DOMImplementation 인터페이스-2: createDocument(), createDocumentType()
**[⬆ 상단으로](#목차)**


## Node 인터페이스

### textContent
### innerText
### outerText
### innerHTML, outerHTML
### Node Tree Position: Node와 Node Tree, Node Tree 포지션 명칭
### insertAdjacentHTML()
### createTextNode(), normalize()
**[⬆ 상단으로](#목차)**


## Node Tree Position 프로퍼티

### 첫 번째 위치 프로퍼티: firstChild, firstElementChild
### 마지막 위치 프로퍼티: lastChild, lastElementChild
### 부모 위치 프로퍼티: parentNode, parentElement
### 다음 형제 위치 프로퍼티: nextSibling, nextElementSibling
### 앞 형제 위치 프로퍼티: previousSibling, previousElementSibling, doctype
**[⬆ 상단으로](#목차)**


## Node Tree 포지션 비교

### compareDocumentPosition()
### contains(), hasChildNodes()
**[⬆ 상단으로](#목차)**


## Node 추가, 삭제, 대체, 복제

### appendChild()
### append(), childElementCount
### insertBefore(), prepend()
### before(), after()
### replaceChild(), replaceChildren(), replaceWith()
### remove(), removeChild(), isConnected
### cloneNode(), isEqualNode()
### importNode(), adoptNode(), ownerDocument
### baseURI, lookupNamespaceURI(), isDefaultNamespace(), lookupPrefix()
**[⬆ 상단으로](#목차)**


## DOM Traversal

### NodeIterator 오브젝트 생성: createNodeIterator(), nextNode()
### NodeIterator 오브젝트 생성: 노드 타입 값, createNodeIterator(), previousNode()
### NodeIterator 오브젝트 프로퍼티: root, whatToShow, referenceNode
### NodeFilter 인터페이스: createNodeIterator(), acceptNode(), filter 프로퍼티
### TreeWalker 인터페이스: createTreeWalker()
### firstChild(), lastChild()
### parentNode(), nextNode(), nextSibling(), previousNode(), previousSibling()
**[⬆ 상단으로](#목차)**


## DocumentFragment 인터페이스

### createDocumentFragment(), DocumentFragment 관련 인터페이스
**[⬆ 상단으로](#목차)**


## 텍스트 처리 인터페이스

### CharacterData 인터페이스-1: appendData(), substringData()
### CharacterData 인터페이스-2: insertData(), replaceData(), deleteData()
### Text 인터페이스: new Text(), splitText()
**[⬆ 상단으로](#목차)**


## HTML 스펙의 Document 인터페이스

### Resource metadata management
### DOM Tree 악세서-1
### DOM Tree 악세서-2: getElementsByName()
### Location 인터페이스: location 프로퍼티
### DOMStringList 인터페이스: ancestorOrigins, item(), contains()
### Location 인터페이스: assign(), replace(), reload()
### dynamic markup insertion: open(), write(), close()
### user interaction: defaultView, designMode, hasFocus(), activeElement
**[⬆ 상단으로](#목차)**


## Window 인터페이스

### current browsing context
### BarProp 인터페이스
### History 인터페이스: back(), forward(), go()
### History 인터페이스: pushState()
### History 인터페이스: replaceState()
### History 인터페이스: scrollRestoration
### other browsing context: WindowProxy, length, frames
### open()
### current browsing context: close(), stop(), focus(), blur()
### other browsing context: parent, top, frameElement, opener
### user prompts: alert(), confirm(), prompt(), print()
**[⬆ 상단으로](#목차)**


## Navigator 인터페이스

### NavigatorID 인터페이스: userAgent
### NavigatorLanguage, NavigatorOnLine, NavigatorCookies 인터페이스
### NavigatorConcurrentHardware, NavigatorContentUtils, originAgentCluster
**[⬆ 상단으로](#목차)**


## Messaging System

### messaging system, postMessage()
### postMessage(): 파라미터 3개 형태
### postMessage()의 transfer
**[⬆ 상단으로](#목차)**


## WindowOrWorkerGlobalScope 인터페이스

### structured cloning: origin, isSecureContext, structuredClone()
### Timers: setTimeout(), clearTimeout(), setInterval(), clearInterval()
### microtask queuing: Call Stack, Event Loop, Task, Task Queue
### microtask queuing: queueMicrotask()
### Base64 utility methods
### ImageBitmap: createImageBitmap()
### ImageBitmap 인터페이스
**[⬆ 상단으로](#목차)**
