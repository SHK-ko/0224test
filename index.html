<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cafe Non-Off Chatbot</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300;400;500;700&display=swap');
        
        body {
            font-family: 'Noto Sans KR', sans-serif;
            background-color: #f3f4f6;
        }

        /* 스크롤바 커스텀 */
        .scrollbar-hide::-webkit-scrollbar {
            display: none;
        }
        .scrollbar-hide {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }

        .chat-bubble {
            max-width: 80%;
            animation: fadeIn 0.3s ease-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .typing-dot {
            animation: typing 1.4s infinite ease-in-out both;
        }
        .typing-dot:nth-child(1) { animation-delay: -0.32s; }
        .typing-dot:nth-child(2) { animation-delay: -0.16s; }
        
        @keyframes typing {
            0%, 80%, 100% { transform: scale(0); }
            40% { transform: scale(1); }
        }
    </style>
</head>
<body class="flex items-center justify-center min-h-screen p-4">

    <!-- 메인 컨테이너 (모바일 앱 스타일) -->
    <div class="w-full max-w-md bg-white rounded-3xl shadow-2xl overflow-hidden flex flex-col h-[800px] max-h-[90vh] border border-gray-200">
        
        <!-- 헤더 -->
        <header class="bg-slate-900 text-white p-4 flex items-center justify-between shadow-md z-10">
            <div class="flex items-center gap-3">
                <div class="w-10 h-10 bg-orange-100 rounded-full flex items-center justify-center text-slate-900 font-bold text-lg">
                    N
                </div>
                <div>
                    <h1 class="font-bold text-lg">Cafe Non-Off</h1>
                    <div class="flex items-center text-xs text-green-400">
                        <span class="w-2 h-2 bg-green-400 rounded-full mr-1 animate-pulse"></span>
                        영업중 (24시간)
                    </div>
                </div>
            </div>
            <button onclick="resetChat()" class="text-gray-300 hover:text-white transition">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M16.023 9.348h4.992v-.001M2.985 19.644v-4.992m0 0h4.992m-4.993 0 13.19-13.19M4.422 4.422l.008.008M4.422 4.422h.002" />
                </svg>
            </button>
        </header>

        <!-- 채팅 영역 -->
        <main id="chat-container" class="flex-1 overflow-y-auto p-4 space-y-4 bg-gray-50 scrollbar-hide">
            <!-- 봇 초기 메시지 -->
            <div class="flex justify-start chat-bubble">
                <div class="bg-white border border-gray-200 text-gray-800 p-4 rounded-2xl rounded-tl-none shadow-sm">
                    <p class="mb-2">안녕하세요! 목동 24시간 브런치 카페 <b>논오프(Non-Off)</b>입니다. ☕️</p>
                    <p>무엇을 도와드릴까요?</p>
                </div>
            </div>
            
            <!-- 퀵 메뉴 버튼 -->
            <div class="grid grid-cols-2 gap-2 text-sm">
                <button onclick="handleKeyword('메뉴')" class="bg-white border border-orange-200 text-orange-600 p-2 rounded-xl hover:bg-orange-50 transition shadow-sm text-left px-3">☕️ 메뉴/가격</button>
                <button onclick="handleKeyword('위치')" class="bg-white border border-orange-200 text-orange-600 p-2 rounded-xl hover:bg-orange-50 transition shadow-sm text-left px-3">📍 위치/주차</button>
                <button onclick="handleKeyword('영업시간')" class="bg-white border border-orange-200 text-orange-600 p-2 rounded-xl hover:bg-orange-50 transition shadow-sm text-left px-3">⏰ 영업시간</button>
                <button onclick="handleKeyword('추천')" class="bg-white border border-orange-200 text-orange-600 p-2 rounded-xl hover:bg-orange-50 transition shadow-sm text-left px-3">👍 추천 메뉴</button>
                <button onclick="handleKeyword('반려동물')" class="bg-white border border-orange-200 text-orange-600 p-2 rounded-xl hover:bg-orange-50 transition shadow-sm text-left px-3">🐶 반려동물</button>
                <button onclick="handleKeyword('와이파이')" class="bg-white border border-orange-200 text-orange-600 p-2 rounded-xl hover:bg-orange-50 transition shadow-sm text-left px-3">📡 와이파이</button>
            </div>
        </main>

        <!-- 입력 영역 -->
        <footer class="p-3 bg-white border-t border-gray-100">
            <form id="chat-form" class="flex gap-2" onsubmit="handleSubmit(event)">
                <input 
                    type="text" 
                    id="user-input" 
                    class="flex-1 bg-gray-100 text-gray-800 rounded-full px-4 py-3 focus:outline-none focus:ring-2 focus:ring-orange-300 transition" 
                    placeholder="궁금한 내용을 입력하세요..."
                    autocomplete="off"
                >
                <button 
                    type="submit" 
                    class="bg-slate-900 text-white rounded-full w-12 h-12 flex items-center justify-center hover:bg-slate-700 transition shadow-lg"
                >
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-5 h-5">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M6 12L3.269 3.126A59.768 59.768 0 0121.485 12 59.77 59.77 0 013.27 20.876L5.999 12zm0 0h7.5" />
                    </svg>
                </button>
            </form>
        </footer>

    </div>

    <script>
        // 카페 데이터베이스 (검색된 정보 기반)
        const cafeData = {
            info: {
                name: "논오프 (Non-Off)",
                address: "서울 양천구 국회대로 279 1층 (목동역 3번 출구 인근)",
                hours: "매일 00:00 - 24:00 (연중무휴)",
                phone: "0507-1344-7009",
                parking: "매장 앞 주차 가능합니다. (공간 여유로운 편)",
                wifi: "ID: Nonoff_5G / PW: nonoffcoffee1!", // 가상의 예시
                pet: "반려동물 동반 가능합니다! 🐶 (테라스 및 실내 일부)",
                toilet: "매장 내 남녀 구분 화장실이 있습니다."
            },
            menu: {
                signature: [
                    { name: "에그 인 헬", price: "8,900원", desc: "매콤한 토마토 소스 브런치" },
                    { name: "프렌치 토스트", price: "7,800원", desc: "촉촉하고 달콤한 인생 토스트" },
                    { name: "가츠산도", price: "8,500원", desc: "두툼한 돈까스 샌드위치" },
                    { name: "소금빵", price: "2,800원~", desc: "기본, 치즈, 대파크림치즈 등 다양" }
                ],
                coffee: [
                    { name: "아메리카노", price: "4,500원" },
                    { name: "카페라떼", price: "5,000원" },
                    { name: "바닐라라떼", price: "5,500원" },
                    { name: "아인슈페너", price: "6,000원" }
                ],
                dessert: [
                    { name: "크로플", price: "변동" },
                    { name: "케이크", price: "변동" }
                ]
            }
        };

        const chatContainer = document.getElementById('chat-container');
        const userInput = document.getElementById('user-input');

        // 메시지 추가 함수
        function addMessage(text, sender, isHtml = false) {
            const wrapper = document.createElement('div');
            wrapper.className = `flex ${sender === 'user' ? 'justify-end' : 'justify-start'} chat-bubble w-full`;
            
            const bubble = document.createElement('div');
            const baseClasses = "p-4 rounded-2xl shadow-sm max-w-[85%] text-sm leading-relaxed";
            
            if (sender === 'user') {
                bubble.className = `${baseClasses} bg-orange-500 text-white rounded-tr-none`;
                bubble.textContent = text;
            } else {
                bubble.className = `${baseClasses} bg-white border border-gray-200 text-gray-800 rounded-tl-none`;
                if (isHtml) {
                    bubble.innerHTML = text;
                } else {
                    bubble.textContent = text;
                }
            }

            wrapper.appendChild(bubble);
            chatContainer.appendChild(wrapper);
            
            // 퀵 메뉴 버튼 뒤로 스크롤
            scrollToBottom();
        }

        // 로딩 표시 함수
        function showLoading() {
            const wrapper = document.createElement('div');
            wrapper.id = 'loading-bubble';
            wrapper.className = 'flex justify-start chat-bubble w-full';
            wrapper.innerHTML = `
                <div class="bg-white border border-gray-200 p-4 rounded-2xl rounded-tl-none shadow-sm flex gap-1">
                    <div class="w-2 h-2 bg-gray-400 rounded-full typing-dot"></div>
                    <div class="w-2 h-2 bg-gray-400 rounded-full typing-dot"></div>
                    <div class="w-2 h-2 bg-gray-400 rounded-full typing-dot"></div>
                </div>
            `;
            chatContainer.appendChild(wrapper);
            scrollToBottom();
        }

        // 로딩 제거 함수
        function removeLoading() {
            const loading = document.getElementById('loading-bubble');
            if (loading) loading.remove();
        }

        function scrollToBottom() {
            chatContainer.scrollTop = chatContainer.scrollHeight;
        }

        // 봇 응답 생성 로직
        function getBotResponse(input) {
            const text = input.toLowerCase().replace(/\s/g, ''); // 공백 제거 및 소문자

            // 1. 메뉴/가격/추천
            if (text.includes('메뉴') || text.includes('가격') || text.includes('얼마') || text.includes('커피') || text.includes('디저트')) {
                let menuHtml = `<p class="font-bold text-lg mb-2">☕️ NON-OFF MENU</p>`;
                
                menuHtml += `<p class="font-bold text-orange-600 mt-2">🌟 시그니처 & 브런치</p><ul class="list-disc pl-4 space-y-1">`;
                cafeData.menu.signature.forEach(m => {
                    menuHtml += `<li><b>${m.name}</b>: ${m.price}</li>`;
                });
                menuHtml += `</ul>`;

                menuHtml += `<p class="font-bold text-orange-600 mt-3">☕️ 커피 & 음료</p><ul class="list-disc pl-4 space-y-1">`;
                cafeData.menu.coffee.slice(0,3).forEach(m => {
                    menuHtml += `<li>${m.name}: ${m.price}</li>`;
                });
                menuHtml += `</ul><p class="text-xs text-gray-400 mt-2">* 더 많은 메뉴는 매장에서 확인해주세요!</p>`;
                
                return menuHtml;
            }

            // 2. 추천
            if (text.includes('추천') || text.includes('인기') || text.includes('맛있는')) {
                return `
                    <p class="font-bold mb-2">👍 논오프 사장님 추천!</p>
                    <p class="mb-2">출출하실 땐 <b class="text-orange-600">에그 인 헬</b>과 <b class="text-orange-600">가츠산도</b>가 인기가 많아요. 🥘</p>
                    <p>달달한게 땡기시면 <b class="text-orange-600">프렌치 토스트</b>나 <b class="text-orange-600">소금빵</b>에 라떼 한 잔 추천드립니다! 🥐</p>
                `;
            }

            // 3. 영업시간
            if (text.includes('시간') || text.includes('영업') || text.includes('언제') || text.includes('닫') || text.includes('휴무')) {
                return `
                    <p class="font-bold text-lg mb-1">⏰ 영업시간 안내</p>
                    <p class="text-xl font-bold text-blue-600">${cafeData.info.hours}</p>
                    <p class="mt-2 text-sm text-gray-600">저희는 24시간 언제나 열려있습니다. 늦은 밤에도 편하게 방문해주세요! 🌙</p>
                `;
            }

            // 4. 위치/주차/가는길
            if (text.includes('위치') || text.includes('주소') || text.includes('어디') || text.includes('주차') || text.includes('차') || text.includes('맵')) {
                return `
                    <p class="font-bold mb-2">📍 위치 & 주차 정보</p>
                    <p class="mb-1"><b>주소:</b> ${cafeData.info.address}</p>
                    <p class="mb-3 text-sm text-gray-500">(목동역 3번 출구에서 가깝습니다)</p>
                    <hr class="my-2 border-gray-200">
                    <p class="font-bold mb-1">🚗 주차</p>
                    <p>${cafeData.info.parking}</p>
                `;
            }

            // 5. 편의시설 (와이파이, 화장실, 콘센트, 노트북)
            if (text.includes('와이파이') || text.includes('비번') || text.includes('wifi')) {
                return `📡 와이파이 정보입니다.<br><b>${cafeData.info.wifi}</b>`;
            }
            
            if (text.includes('화장실')) {
                return `🚻 ${cafeData.info.toilet}`;
            }

            if (text.includes('콘센트') || text.includes('노트북') || text.includes('공부') || text.includes('스터디')) {
                return `💻 네! 노트북하기 좋은 넓은 테이블과 콘센트가 넉넉히 준비되어 있습니다. 카공(카페 공부) 환영해요!`;
            }

            // 6. 반려동물
            if (text.includes('개') || text.includes('강아지') || text.includes('고양이') || text.includes('애견') || text.includes('반려') || text.includes('펫')) {
                return `🐶 <b>${cafeData.info.pet}</b><br>사랑하는 댕댕이와 함께 오셔서 테라스의 낭만을 즐겨보세요!`;
            }

            // 7. 전화
            if (text.includes('전화') || text.includes('번호') || text.includes('연락')) {
                return `📞 매장 전화번호는 <b>${cafeData.info.phone}</b> 입니다.`;
            }

            // 8. 인사
            if (text.includes('안녕') || text.includes('반가')) {
                return `안녕하세요! 오늘도 논오프를 찾아주셔서 감사합니다. 😊 커피 한 잔 어떠세요?`;
            }

             // 9. 감사
             if (text.includes('고마') || text.includes('감사') || text.includes('땡큐')) {
                return `도움이 되어서 기쁘네요! 매장에서 뵙겠습니다. 🥰`;
            }

            // 기본 응답
            return `
                죄송해요, 제가 잘 모르는 내용이에요. 😅<br>
                <br>
                - <b>메뉴, 영업시간, 위치, 주차</b> 등에 대해 물어봐 주세요.<br>
                - 기타 문의는 매장으로 전화 주시면 친절히 안내해 드릴게요!<br>
                📞 <a href="tel:${cafeData.info.phone}" class="text-blue-500 underline">${cafeData.info.phone}</a>
            `;
        }

        // 키워드 핸들러 (버튼 클릭용)
        function handleKeyword(keyword) {
            handleSubmit(null, keyword);
        }

        // 전송 핸들러
        async function handleSubmit(event, keyword = null) {
            if (event) event.preventDefault();
            
            const text = keyword || userInput.value.trim();
            if (!text) return;

            // 사용자 메시지 표시
            addMessage(text, 'user');
            userInput.value = '';

            // 로딩 표시
            showLoading();

            // 봇 응답 지연 시뮬레이션 (자연스러움)
            setTimeout(() => {
                removeLoading();
                const response = getBotResponse(text);
                addMessage(response, 'bot', true);
            }, 600 + Math.random() * 500);
        }

        function resetChat() {
            const bubbles = document.querySelectorAll('.chat-bubble');
            // 첫 번째(인사말)과 퀵 버튼을 제외하고 삭제하려면 인덱스 조정 필요하지만,
            // 간단하게 리로드하거나 내용을 비우고 초기 메시지만 다시 넣습니다.
            chatContainer.innerHTML = '';
            
            // 초기 메시지 복구
            const initialMsg = document.createElement('div');
            initialMsg.className = "flex justify-start chat-bubble";
            initialMsg.innerHTML = `
                <div class="bg-white border border-gray-200 text-gray-800 p-4 rounded-2xl rounded-tl-none shadow-sm">
                    <p class="mb-2">안녕하세요! 목동 24시간 브런치 카페 <b>논오프(Non-Off)</b>입니다. ☕️</p>
                    <p>초기화 되었습니다. 무엇을 도와드릴까요?</p>
                </div>
            `;
            chatContainer.appendChild(initialMsg);
            
            // 퀵메뉴 버튼 복구 (HTML 문자열로 다시 삽입)
            const quickMenu = document.createElement('div');
            quickMenu.className = "grid grid-cols-2 gap-2 text-sm";
            quickMenu.innerHTML = `
                <button onclick="handleKeyword('메뉴')" class="bg-white border border-orange-200 text-orange-600 p-2 rounded-xl hover:bg-orange-50 transition shadow-sm text-left px-3">☕️ 메뉴/가격</button>
                <button onclick="handleKeyword('위치')" class="bg-white border border-orange-200 text-orange-600 p-2 rounded-xl hover:bg-orange-50 transition shadow-sm text-left px-3">📍 위치/주차</button>
                <button onclick="handleKeyword('영업시간')" class="bg-white border border-orange-200 text-orange-600 p-2 rounded-xl hover:bg-orange-50 transition shadow-sm text-left px-3">⏰ 영업시간</button>
                <button onclick="handleKeyword('추천')" class="bg-white border border-orange-200 text-orange-600 p-2 rounded-xl hover:bg-orange-50 transition shadow-sm text-left px-3">👍 추천 메뉴</button>
                <button onclick="handleKeyword('반려동물')" class="bg-white border border-orange-200 text-orange-600 p-2 rounded-xl hover:bg-orange-50 transition shadow-sm text-left px-3">🐶 반려동물</button>
                <button onclick="handleKeyword('와이파이')" class="bg-white border border-orange-200 text-orange-600 p-2 rounded-xl hover:bg-orange-50 transition shadow-sm text-left px-3">📡 와이파이</button>
            `;
            chatContainer.appendChild(quickMenu);
        }
    </script>
</body>
</html>
