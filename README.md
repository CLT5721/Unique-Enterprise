# Unique-remitone8888
 將 iOSApp 送審上架到 AppStore
 使用Xcode打開App專案，將App上傳到App Store Connect，設置App在App Store的名稱參考以下鏈接的說明，將App上傳到App Store Connect。
將 App 上傳到 App Store Connect寫了上千行的 Swift 程序，辛苦開發完成 App 後，距離目標上架 App Store，剩下兩個空間任務要完成：
上傳過程中，在Preparing app record視窗設置的Name將成為App in App Store的名稱，這裡我們輸入ReadIn Blog。
連接到App Store Connect網站設置App 資訊   點選上圖向右的箭頭或以下網址。
http://appstoreconnect.apple.com
點選想要設定的App
點選剛剛上傳的App ReadIn Blog。
進入App的設定頁面。
上傳應用程序畫面的圖片和視頻（應用程序預覽和屏幕截圖）
切換到App Store的準備提交頁面，從App預覽和屏幕截圖上傳App的圖片和視頻。
格式為JPG或PNG。雖然iPhone有多種尺寸，不過我們只需上傳6.5 & 5.5寸的圖片。關於如何製作上架所需的圖片，可參考以下鏈接。
如何生成符合上架尺寸的截圖（螢幕截圖）當我們準備上架iPhone App時，需要上傳App的螢幕截圖，而且圖片的尺寸要跟真正的iPhone一模一樣，差一個像素都不行。
若想進一步設計吸睛的App圖片，想要有漂亮的iPhone外框和文字說明，可參考以下鏈接的說明。
為 iOS App 畫面加上美美的 iPhone 外框 (frame) 和文字說明
很多App Store的截圖都是結合iPhone外框圖片和文字說明，比方以下FB Messenger的例子：
如果App也有iPad版本，則需再上傳iPad Pro (3rd Gen) 12.9 & iPad Pro (2nd Gen) 12.9的圖片。
從TARGETS App General頁面的部署信息區塊可查詢App是否同時包含iPhone & iPad版本，目前Xcode 默認創建的新專案會同時勾選iPhone 和iPad。
設定行銷宣傳文字和描述(Promotional Text & Description)促銷文字和說明
行銷宣傳文字和描述是App的文字介紹，雖然大部分的用戶都不會看，我們還是用心用愛好好地寫。
就像在 App Store 的準備提交頁面一樣，從促銷文本和描述設置行銷宣傳文字和描述。
描述，行銷宣傳文字有好處，它可以隨時修改更新。正好，App一旦上架，描述只能等新版本送審時更新。
設定App的關鍵字，支持URL和行銷URL( Keywords，Support URL，Marketing URL)
設為公司的網站。
在App Store的應用頁面，開發者網站（開發者網站）將對應行銷URL。
此版本必須與 ***Xcode 專案裡設定的 App 版本 (Version) ***一致。當我們從 Xcode 上傳 App 時，網頁上的版本會自動設為與專案一致，因此通常不需要另外設定。
設定版權(Copyright)
應用程序就像我們懷胎十月生出的寶寶，當然要設定版權，聲明版權我們所有。
設定登入資訊
有些App需要登入才能使用，為了讓偉大的Apple評審大不用麻煩地重新註冊帳號，
我們可以在App Review信息下提供一組帳號密碼。
