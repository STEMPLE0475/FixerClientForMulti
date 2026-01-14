# FixerClientForMulti
Fixer 멀티플레이 구현에 사용된 클라이언트 코드

# 주요 코드 설명
NetPlayerManager : (Singleton) 방에 접속되어 있는 모든 플레이어를 관리
NetPlayerObjectManager : MultiPlay Scene에서 NetPlayerManager의 정보를 받아 NetPlayer(다른 플레이어)의 오브젝트를 생성/관리
Packet.proto : 서버와 동일한 패킷을 사용하기 위해서 코드를 생성하기 위한 설계도 (실제 사용시, 이 파일을 기반으로 코드 생성)
FixerClient : (Singleton) 서버와 연결을 위한 핵심 클래스
FixerPacketHandler : 서버 패킷을 받아 실행되는 함수를 담는 클래스
FixerClientService : 서버에 요청을 하는 함수를 담는 클래스
