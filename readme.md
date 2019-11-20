
# 오픈소스SW의 성당과 시장 모델
  1. 성당모델: 일찍, 그리고 자주 발표하며 다른 사람에게 위임할 수 있는 것은 모두 위임하고, 뒤범벅된 부분까지 공개하는 개발 방식
  
  2. 시장모델: 뛰어난 프로그래머에 의해서 조심스럽게 개발되는 방식
  
# 지적 재산권과 라이선스
  1. 지적재산권: SW는 지적 재산권으로부터 보호를 받고 있고, 지적재산권은 저작권, 특허권, 상표권, 영업비밀 등으로 구성됨
  
    * 저작권: 어떠한 절차나 형식의 이행을 필요로 하지 아니함
    * 특허권: 자연적으로 부여되지 않으며, 특허청에 출원하여 심사를 받고 설정등록을 해야만 권리가 발생함
    * 상표권: 상표등록을 출원하여 심사를 받고 설정등록을 해야 권리가 생김
  
  2. 라이선스: SW 저작권자와 사용자간의 이용방법 및 조건의 범위 정의해 놓은 허가권임
  
    * FOSS 라이선스는 크게 반환의무가 있는 라이선스와 반환이 불필요한 라이선스로 나뉘어짐
    * 반환의무가 있는 라이선스의 대표적인 예로는 GPL이 존재함
    * 반환이 불필요한 라이선스의 대표적인 예로는 MPL이 존재함
    * 원작자가 배포한 코드가 반환의무가 없는 라이선스를 사용하고 있다면, 수정된 코드는 반드시 동일한 라이선스를 
      적용하여 배포되어야 함
    
  3. GPL 라이선스
  
    * GPL 2.0은 SW 특허 문제와 설치정보와 관련된 문제(DRM)으로 인해 GPL 3.0 으로 개정되었음
    * GPL 3.0에서는 라이선스에 포함된 특허의 권리를 양도하는 patent grant와 라이선스 규정을 어겼을 때 발동하는 
      patent retailiation 조항이 있음
    * GPL 2.0, 3.0 모두 모든 derived work의 소스코드 공개를 요구함


# 오픈소스 거버넌스
   
   1. 공개 SW의 기술 및 의무사항에 대한 이해 부족으로 오픈소스 사용에는 기술적인 위험, 운영적인 위험, 법적인 위험 등이 존재함
   
   2. 이러한 리스크를 관리하기 위해서 오픈소스 거버넌스가 필요함


# Git 기본 명령어
  1. Git의 작업 공간은 크게 관리 대상인 파일과 관리대상이 아닌 파일으로 나뉘어져 있음
  
  2. Git add 명령어는 작업폴더에서 수정된 내용을 stage에 올리고, commit 명령어는 stage에 올려진 파일을 로컬 .git derectory에 저장함
  
  3. Push 명령어는 로컬에서 업데이트 된 내용들을, 원격 저장소에 업로드하는 명령어임
  
  4. Pull 명령어와 Fetch 명령어는 원격지로부터 업데이트된 파일을 로컬에 다운받는 것이고, Pull과 달리 Fetch는 다운받은 후 Merge도 수행함
  
  5. SSH 키를 원격 저장소에 등록하면, 해당 저장소의 SSH 주소를 동해 원격 저장소의 접근 및 복사가 가능하고, 원격저장소에 write를 수행할 수 있음
  
  
# 오픈소스와 정보보호

  1. 오픈소스 보안 기술을 활용하면 기존의 상용 보안 기술보다 시스템을 보다 안전하게 운영할 수 있음
  
  2. JAVA 기반 오픈소스 암호 라이브러리는 대표적으로 Bouncycastle이 많이 사용됨
  
    * Bouncycastle에는 다양한 암호알고리즘이 존재함
    * Bouncycastle에는 암호학적 해쉬 함수들이 존재하고, 특정 input에 대한 암호학적 해쉬함수 결과값을 만들기 위해서는 
      항상 update함수와 Digest함수를 사용해야 함
    
