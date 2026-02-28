# -// ส่วนของการประกาศตัวแปรสถานะ (เปิด/ปิด)
bool aimbot_head = false;
bool anti_ban = false;

// ฟังก์ชันสำหรับวาดหน้าเมนู (UI Render)
void RenderModMenu() {
    // เริ่มสร้างหน้าต่างเมนู
    ImGui::Begin("My Custom Mod Menu", nullptr, ImGuiWindowFlags_AlwaysAutoResize);

    ImGui::Text("เลือกฟังก์ชันที่ต้องการใช้งาน:");
    ImGui::Separator();

    // 1. ฟังก์ชันดูดหัว (Checkbox สำหรับเปิด-ปิด)
    if (ImGui::Checkbox("1. ดูดหัว 99% (Aimbot)", &aimbot_head)) {
        // เมื่อกดติ๊กถูก ระบบจะเปลี่ยนค่า aimbot_head เป็น true หรือ false
    }

    // 2. ฟังก์ชันกันแบน (Checkbox สำหรับเปิด-ปิด)
    if (ImGui::Checkbox("2. กันแบน 100% (Anti-Ban)", &anti_ban)) {
        // เมื่อกดติ๊กถูก ระบบจะเปลี่ยนค่า anti_ban เป็น true หรือ false
    }

    ImGui::Separator();
    if (ImGui::Button("ปิดเมนู")) {
        // โค้ดสำหรับซ่อนเมนู
    }

    ImGui::End();
}

// ส่วนของ Logic การทำงาน (ตัวอย่างคร่าวๆ)
void GameLoop() {
    if (aimbot_head) {
        // ใส่ Code สำหรับการคำนวณตำแหน่งหัวและเลื่อนเป้าไปที่นั่น (Memory Writing/Hooking)
    }
    
    if (anti_ban) {
        // ใส่ Code สำหรับการ Bypass ระบบป้องกันของเกม
    }
}
