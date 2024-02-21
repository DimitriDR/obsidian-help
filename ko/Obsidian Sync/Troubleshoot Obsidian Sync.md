이 페이지에서는 만날 수 있는 일반적인 문제와 그 문제를 해결하는 방법을 나열하고 있습니다.

## Conflict resolution

두 대 이상의 장치에서 동기화 사이에 동일한 파일을 변경하면 충돌이 발생합니다.예를 들어, 컴퓨터에서 파일을 변경한 후 해당 변경 사항이 업로드되기 전에 핸드폰에서도 동일한 파일을 변경했을 수 있습니다.

일반적으로 오프라인에서 작업하는 경우 충돌이 더 자주 발생합니다. 이는 더 많은 변경 사항과 동기화 간의 더 긴 시간 간격 때문에 더 많은 잠재적인 충돌이 발생하기 때문입니다.

동기화가 파일의 새 버전을 다운로드하고 로컬 버전과 충돌이 발견될때 변경 사항이 Google의 diff-match-patch 알고리즘으로 병합됩니다.

> [!tip]
> 충돌이 발생한 경우를 찾으려면 **설정 → 동기화 → 동기화 활동 → 열람**에서 "충돌 파일 병합 중"을 검색할 수 있습니다.

# Obsidian Sync deleted a note I just created on two devices

일반적으로, Obsidian Sync는 충돌하는 노트의 내용을 병합하여 장치간의 [[#Conflict resolution|충돌을 해결]]하려고 시도합니다.안타깝게도 충돌하는 노트를 병합하면 시작 시 자동으로 노트를 생성하거나 변경하는 사용자에게 문제가 발생할 수 있습니다. 예를 들어 데일리 노트를 사용하는 경우.

원격 버전 노트를 동기화 다운로드 전 2분 미만에 디바이스에 노트가 로컬로 생성되었다면, 동기화는 그 노트를 병합하지 않고 원격 버전을 유지합니다. 여전히 [[File recovery|파일 복구]]를 사용하여 로컬 버전을 복구할 수 있습니다.

## What does the `vault limit exceeded` error mean?

보관소가 [[Limitations#How large can each remote vault be|최대 10GB 크기 제한]]을 초과합니다. [[Remote vault size limit|원격 보관소 사이즈 제한]]을 참조하십시오.

첨부 파일과 버전 기록이 보관소의 총 크기에 관여하기 때문에 실제 보관소의 크기가 제한보다 작더라도 최대 크기보다 큰 경우가 있을 수 있습니다.

보관소에서 큰 파일을 식별하고 삭제하려면:

1. **설정 → 동기화**을 엽니다.
2. 보관소 크기를 줄이는 방법에 대한 **보관소의 허용 크기** 아래의 옵션을 탐색합니다.