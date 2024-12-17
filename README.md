# Calculator

by Athiwat Tangrusicharoen,
673450041-1,
Computer and Infomation Science, KKU

# การรับและการแสดงผลข้อมูล

รับข้อมูลจากผู้ใช้งาน และทำงานผ่านการกดปุ่มเพื่อคำนวนตัวเลข

## ปุ่มบวก

private void button1_Click(object sender, EventArgs e)
{
    // ข้อความตัวอักษร
    // str / string = ต่าที่เป็นข้อความ
    string inputNum1 = num1.Text;
    string inputNum2 = num2.Text;
    // convert string to number (integer)
    // double / float = ใส่ค่าเลขตัแปรเป็นทศนิยมได้
    double iNum1 = double.Parse(inputNum1);
    double iNum2 = double.Parse(inputNum2);
    // double ทำให้เราสามารถ + - * / ได้
    double iResult = iNum1 + iNum2;
    // ที่ตัวแปรชื่อ result
    // มีคุณสมบัติชื่อ Text
    result.Text = iResult.ToString(); // .ToString = แปรค่าเป็น str
}
