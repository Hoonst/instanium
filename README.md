# instanium
Code for Crawling Instagram by Selenium

해당 코드들은 Instagram의 데이터들을 '#' 해시태그를 기준으로 뽑아오는 것입니다.

일반인이 인스타그램 API에 직접 접근하여 Token을 받는 것은 거의 불가능하다고 판단했기에
Selenium을 사용했으며 chrome driver를 사용하여 데이터를 가져와습니다.

두 가지 코드가 있으니 Scroll_version --> Access_version 순으로 진행해주시길 바랍니다.

Scroll_version:
인스타그램의 각 게시물이 개별 주소를 가져오는 것입니다.
따라서 스크롤을 아래로 계속 진행하면서 HTML을 가져오고 각 링크를 가져온 후 Flush를 시킨 후
다시 스크롤을 내려가면서 반복합니다.

Access_version:
위에서 가져온 link에 하나씩 들어가서 원하는 데이터(시간, 게시글, 사진 주소 etc 개별 설정 가능)를 가져옵니다.

** 만들고 바로 실행했을 때는 원활하게 데이터를 가져올 수 있었으나 요즘들어 에러가 발생하는 것 같으니
** Custom이 필요할 것 같으며 이것은 코드의 문제라기보다 Instagram 자체의 변화때문에 발생하는 듯 합니다.

