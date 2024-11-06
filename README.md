# ChainGate
사용자 관리
login_view: 사용자 ID와 비밀번호를 확인하여 인증하는 함수입니다. 로그인 정보가 일치하면 세션에 사용자 이름을 저장하고 방문자 검색 페이지로 리디렉션합니다. 일치하지 않으면 오류 메시지를 표시합니다.

search_user: 이름과 부서를 기준으로 사용자 정보를 검색하고, user_id가 주어진 경우 해당 사용자의 세부 정보를 추가로 조회합니다.

create_user: 새로운 사용자를 추가하는 페이지를 렌더링합니다.

update_user: user_id에 해당하는 사용자의 세부 정보를 조회하고, 수정 페이지에 표시합니다.

save_user: 사용자 정보를 저장하는 함수입니다. 주어진 user_id가 존재하면 사용자의 정보를 업데이트하고, 사진이 첨부된 경우 사진 경로를 저장합니다.

delete_user: 특정 user_id를 가진 사용자를 삭제하는 함수입니다.

insert_user: 새로운 사용자를 데이터베이스에 추가하는 함수입니다. 사진 파일이 첨부되면 파일 경로를 저장합니다.

방문자 관리
search_visitor: 방문자를 이름과 부서를 기준으로 검색하며, visitor_id가 제공되면 해당 방문자의 세부 정보를 조회합니다.

create_visitor: 새로운 방문자를 추가하는 페이지를 렌더링합니다.

update_visitor: 특정 visitor_id에 해당하는 방문자의 세부 정보를 조회하고, 수정 페이지에 표시합니다.

save_visitor: 방문자 정보를 저장하는 함수입니다. 주어진 visitor_id에 해당하는 정보를 업데이트하며, 사진이 첨부된 경우 파일 경로를 저장합니다.

delete_visitor: 지문 정보와 함께 방문자 데이터를 삭제하는 함수입니다. 지문 삭제가 성공하면 방문자 정보도 삭제됩니다.

insert_visitor: 새로운 방문자를 데이터베이스에 추가하는 함수로, 사진이 첨부된 경우 파일 경로를 저장합니다.

출입 로그 및 기타
entrance_log: 출입 로그를 조회하는 함수로, 날짜, 이름, 부서별로 검색이 가능합니다. 세부 정보 조회를 위해 employee_id에 해당하는 방문자 정보를 가져올 수 있습니다.

enroll_fingerprint: 사번을 기준으로 지문 등록을 요청하는 함수입니다. 지문 등록이 성공하면 성공 메시지를 반환합니다.

approve_entry: 지문 인식을 통해 출입을 승인하는 함수입니다. 지문 인식이 성공하면 방문자의 정보를 조회하고, 블록체인에 출입 정보를 기록합니다.

각 함수는 특정한 입력이나 데이터베이스 처리를 기반으로 출입 및 사용자/방문자 관리를 위한 다양한 기능을 수행하고 있습니다.