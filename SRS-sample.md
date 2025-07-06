아래는 기능 요구사항과 비기능 요구사항에 샘플입니다.  

| 구성 요소                                   | 요구사항 내용                                                                                     | 검증 내용                                                                                     |
|------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| 1. 소개 (Introduction)                   | 이 문서는 소프트웨어 시스템의 요구사항을 정의하기 위해 작성되었다.                                   | 요구사항 정의서가 이해관계자에게 명확하게 전달되었는지 확인한다.                                   |
| 1.1 목적 (Purpose)                       | 이 요구사항 정의서는 개발자와 이해관계자 간의 명확한 소통을 위해 필요하다.                           | 요구사항의 목적이 모든 이해관계자에게 이해되었는지 검증한다.                                   |
| 1.2 범위 (Scope)                         | 본 시스템은 사용자 관리, 데이터 처리 및 보고서 생성 기능을 포함한다.                               | 시스템의 범위가 명확히 정의되었는지 확인하고, 모든 기능이 포함되었는지 검증한다.                     |
| 2. 기능 요구사항 (Functional Requirements) | 시스템이 제공해야 하는 기능을 정의한다.                                                            | 각 기능이 요구사항에 맞게 구현되었는지 확인하기 위해 테스트 케이스를 작성하고 실행한다.               |
| 2.1 사용자 로그인 (User Login)          | 사용자는 이메일과 비밀번호를 입력하여 시스템에 로그인할 수 있어야 하며, 로그인 실패 시 오류 메시지를 표시해야 한다. | 유효한 이메일과 비밀번호로 로그인 시도 후 성공 여부 및 오류 메시지 확인 테스트를 수행한다.             |
| 2.2 데이터 입력 (Data Input)            | 사용자는 데이터를 입력하고 저장할 수 있어야 하며, 입력된 데이터는 데이터베이스에 저장된다. 데이터 입력 시 필수 항목은 이름, 이메일, 전화번호이다. | 필수 항목을 입력 후 저장하고, 데이터베이스에서 입력된 데이터가 정확히 저장되었는지 확인한다.         |
| 2.3 보고서 생성 (Report Generation)     | 사용자는 입력된 데이터를 기반으로 다양한 형식의 보고서를 생성할 수 있어야 하며, 보고서는 PDF 및 Excel 형식으로 다운로드 가능해야 한다. | 보고서 생성 후 다운로드하여 형식이 올바른지 및 데이터가 정확한지 검증한다.                           |
| 3. 비기능 요구사항 (Non-functional Requirements) | 시스템의 품질 속성을 정의한다.                                                                    | 비기능 요구사항이 충족되었는지 확인하기 위해 성능 테스트 및 보안 테스트를 수행한다.                   |
| 3.1 성능 (Performance)                   | 시스템은 1000명의 동시 사용자를 지원할 수 있어야 하며, 응답 시간은 2초 이내여야 한다.               | 부하 테스트 도구를 사용하여 동시 사용자 수를 증가시키며 응답 시간을 측정한다.                       |
| 3.2 보안 (Security)                      | 모든 사용자 데이터는 AES-256 암호화 방식으로 저장되어야 하며, 비밀번호는 최소 8자 이상, 대문자, 소문자, 숫자 및 특수문자를 포함해야 한다. | 데이터베이스에서 암호화된 비밀번호를 확인하고, 비밀번호 정책을 테스트하여 요구사항 충족 여부를 검증한다. |
| 3.3 사용성 (Usability)                   | 시스템은 직관적인 사용자 인터페이스를 제공해야 하며, 사용자는 5분 이내에 기본 기능을 익힐 수 있어야 한다. | 사용자 테스트를 통해 실제 사용자가 시스템을 사용해보도록 하고, 기능 익히는 데 걸리는 시간을 측정한다.   |
| 4. 제약 사항 (Constraints)               | 시스템은 특정 하드웨어(예: Intel i5 이상) 및 소프트웨어 환경(예: Windows 10 이상)에서만 작동해야 하며, 법적 규제를 준수해야 한다. | 시스템이 요구하는 하드웨어 및 소프트웨어 환경에서 정상적으로 작동하는지 확인한다.                     |
| 5. 검증 (Verification)                   | 모든 요구사항은 테스트 케이스를 통해 검증되어야 하며, 검증 방법은 문서화되어야 한다. 각 기능 요구사항에 대해 최소 2개의 테스트 케이스가 필요하다. | 각 요구사항에 대한 테스트 케이스를 작성하고, 단계별 테스트 및 인수 테스트에서 활용하여 검증한다.       |

이 표는 각 요구사항에 대한 검증 내용을 구체적으로 업데이트하여, 요구사항이 충족되는지를 명확히 확인할 수 있도록 구성되었습니다. 각 검증 방법은 요구사항의 품질을 보장하고, 개발 과정에서 발생할 수 있는 리스크를 줄이는 데 중요한 역할을 합니다.
[1] https://velog.io/@y55nms/4.-%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD  
[2] https://born-better.tistory.com/4  
[3] https://swingswing.tistory.com/253  
[4] https://blog.naver.com/sharon0a/110048676563?viewType=pc  
[5] https://codingpineapple.com/entry/%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4%EA%B0%9C%EB%B0%9C-%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD%EB%B6%84%EC%84%9D-%EB%B9%84%EA%B8%B0%EB%8A%A5%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD-%EA%B8%B0%EB%8A%A5%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD  
[6] https://howudong.tistory.com/78  
[7] https://blog.naver.com/wisestone2007/223338290965?viewType=pc  
[8] https://serviceable.tistory.com/entry/%EC%A0%95%EC%B2%98%EA%B8%B0-%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD-%EB%B6%84%EC%84%9D%EA%B8%B0%EB%B2%95  
[9] https://ee-22-joo.tistory.com/2  
[10] https://www.requiment.com/the-importance-of-updating-requirement-documentation-throughout-a-project/  
[11] https://work-01.tistory.com/285  
[12] https://annyeongworld.tistory.com/entry/%EA%B8%B0%EB%8A%A5%EC%A0%81-%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD%EA%B3%BC-%EB%B9%84%EA%B8%B0%EB%8A%A5%EC%A0%81-%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD  
[13] https://velog.io/@seola1ne/%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD%EA%B3%BC-%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD-%EC%97%94%EC%A7%80%EB%8B%88%EC%96%B4%EB%A7%81  
[14] https://simple-cha.tistory.com/5  
[15] https://www.requiment.com/how-to-write-a-software-requirements-document-srd/  
[16] https://m.blog.naver.com/wishket/223492840973   
[17] https://ggumidr.com/entry/%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD-%EC%A0%95%EC%9D%98%EC%84%9CSoftware-Requirements-Specification  
[18] https://visuresolutions.com/ko/%EC%9A%94%EA%B5%AC-%EC%82%AC%ED%95%AD-%EA%B4%80%EB%A6%AC-%EC%B6%94%EC%A0%81%EC%84%B1-%EA%B0%80%EC%9D%B4%EB%93%9C/%EB%B9%84-%EA%B8%B0%EB%8A%A5%EC%A0%81-%EC%9A%94%EA%B5%AC-%EC%82%AC%ED%95%AD/  
[19] https://tonyjev93.github.io/software%20engineering/requirements-analysis/  
[20] https://www.geeksforgeeks.org/software-requirement-specification-srs-format/  
[21] https://www.modernrequirements.com/blogs/requirements-specification/  
[22] https://www.jamasoftware.com/requirements-management-guide/writing-requirements/how-to-write-system-requirement-specification-srs-documents/  
[23] https://m.blog.naver.com/hann726/222021461073  
[24] https://www.codestates.com/blog/content/prd-%EC%A0%9C%ED%92%88%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD%EC%A0%95%EC%9D%98%EC%84%9C  
[25] https://anajane.tistory.com/entry/%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD%EC%A0%95%EC%9D%98%EC%84%9C-%EA%B4%80%EB%A6%AC-%EC%B6%94%EA%B0%80-%EA%B8%B0%EB%8A%A5-%EB%8F%84%EC%B6%9C%EA%B3%BC-%EC%82%AD%EC%A0%9C-%EB%B0%A9%EB%B2%95  
[26] https://document360.com/blog/software-requirements-document/  
[27] https://velog.io/@juyeon/%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD-%EC%A0%95%EC%9D%98%EC%84%9C-%EC%9E%91%EC%84%B1%ED%95%98%EB%8A%94-%EB%B2%95  
[28] https://whatilearned.tistory.com/147  
[29] https://eun-developer.tistory.com/102  
[30] https://velog.io/@bagt/%EC%82%AC%EC%9A%A9%EC%9E%90-%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD-%EC%A0%95%EC%9D%98%EC%84%9C-SRS%EB%9E%80  
[31] https://blog.naver.com/wishket/223530339068  
[32] https://www.perforce.com/blog/alm/how-write-software-requirements-specification-srs-document  
[33] https://asana.com/resources/software-requirement-document-template  
[34] https://pm.stackexchange.com/questions/9279/does-a-change-request-change-the-requirement-specification  
[35] https://www.linkedin.com/advice/3/how-do-you-update-system-requirements-specifications  
