---
layout: post
title: 'dappTunes'
---

## 학원에서의 마지막 프로젝트는 [기업협약](#) 으로 [MetaTrend](#) 와 함께 진행 한 [음원 nft 마켓](#) 입니다.

프로젝트 기획 초기, youtube, spotify, melon 과 같이 중앙화 하여 음원소스를 관리하는 것은 

자유로운 고객, 아티스트들의 탈중앙화 니즈를 충족 시켜줄수 없다 판단되어, 

[블록체인](#)과 [ERC-721 토큰](#)의 특성을 사용해 모든 사용자들이 [자유롭게](#) 등록,판매,실행하는 음원 NFT 마켓을 구상했습니다.

전 프로젝트와 다르게 배포시 [aws](#) 대신 [serverLess](#)인 [vercel](#)을 사용해 배포작업 기간을 줄였고, 

이에 따라 [gitflow](#), [gitAction](#) 로 쉽게 빌드배포 테스트를 할수 있게 했습니다.

상용 되는 [ERC-721 token](#) 을 참고해, 음원을 토큰화 하여 [pinata Cloud](#), [google Cloud](#)에 각각 앨범커버와 음원파일을 등록하고,

경매시스템을 구축해 [web3](#) 라이브러리로 서로 다른 [contract](#) (minting , auction) 를 연결시킨 것은 매우 뿌듯했습니다.

아쉬운 점 첫번째로 프론트에서 [redux tool kit](#) 사용이 있었습니다.

프로젝트의 전체적인 볼륨에 비해 무겁고 복잡한 것이 단점이였습니다.

이에 따라 depth 가 깊지 않음에도 [Slice](#) 사용 위치를 찾는 것이 어려웠습니다. 

다음 프로젝트에는 대신 [SWR](#) 을 활용해 [react](#) 전역 상태 관리를 더 쉽게 만드는 도전을 해볼 예정입니다.

{% include image.html image="projects/proj-4/dappTunes1.png" %}

[metamask](#) 의 [window.eth](#) 를 사용해 웹사이트 접속시 이메일 만으로 자동 로그인 되도록 했습니다.

모든 [rpc 요청](#)을 프론트와 백에서 나누어 처리하여 의도한대로 컨트랙트의 발동을 시켰습니다. 

[getStatic](#) 함수사용으로 클라이언트에게 빈 화면을 보여주는 것을 최소화 했으며,

[SEO](#) 검색 처리를 통해 [SSR](#)의 장점을 두각시키고자 노력했습니다.

{% include image.html image="projects/proj-4/dappTunes4.png" %}

음원 토큰 민팅시에 [토큰ID](#)를 네트워크에 등록시킴으로,

최소한의 db 만 가지고도 토큰의 관리가 용이했습니다.

이 점은 클라이언트 들에게 있어 비용절감을 하게 해주는 효과를 보게 해줄것 으로 예상됩니다.

{% include image.html image="projects/proj-4/dappTunes2.png" %}

{% include image.html image="projects/proj-4/dappTunes5.png" %}

{% include image.html image="projects/proj-4/dappTunes3.png" %}

마켓에 경매 contract 를 발동 시킨 모습입니다.

입찰자가 없을 경우에는 언제든지 경매취소를 할 수 있었으며,

경매 완료시 입찰에 들어간 화폐를 경매 등록자, 입찰 실패자 에게 되돌려주고

음원 토큰의 권한을 경매를 성공한 사람에게 위임을 해주었습니다.



