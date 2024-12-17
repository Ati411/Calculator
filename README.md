# Calculator

by Athiwat Tangrusicharoen,
673450041-1,
Computer and Infomation Science, KKU

namespace Winform
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void label1_Click(object sender, EventArgs e)
        {

        }

        private void result_TextChanged(object sender, EventArgs e)
        {

        }

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

        private void button2_Click(object sender, EventArgs e)
        {
            // ข้อความตัวอักษร
            string inputNum1 = num1.Text;
            string inputNum2 = num2.Text;
            // convert string to number (integer)
            // int / integer = ใส่ค่าตัวเลขเป็นจำนวนเต็ม
            int iNum1 = Int32.Parse(inputNum1);
            int iNum2 = Int32.Parse(inputNum2);
            // int ทำให้เราสามารถ + - * / ได้
            int iResult = iNum1 - iNum2;
            // ที่ตัวแปรชื่อ result
            // มีคุณสมบัติชื่อ Text
            result.Text = iResult.ToString(); // .ToString = แปรค่าเป็น str
        }

        private void button3_Click(object sender, EventArgs e)
        {
            // ข้อความตัวอักษร
            string inputNum1 = num1.Text;
            string inputNum2 = num2.Text;
            // convert string to number (integer)
            // int / integer = ใส่ค่าตัวเลขเป็นจำนวนเต็ม
            int iNum1 = Int32.Parse(inputNum1);
            int iNum2 = Int32.Parse(inputNum2);
            // int ทำให้เราสามารถ + - * / ได้
            int iResult = iNum1 * iNum2;
            // ที่ตัวแปรชื่อ result
            // มีคุณสมบัติชื่อ Text
            result.Text = iResult.ToString(); // .ToString = แปรค่าเป็น str
        }

        private void button4_Click(object sender, EventArgs e)
        {
            // ข้อความตัวอักษร
            string inputNum1 = num1.Text;
            string inputNum2 = num2.Text;
            // convert string to number (integer)
            // int / integer = ใส่ค่าตัวเลขเป็นจำนวนเต็ม
            int iNum1 = Int32.Parse(inputNum1);
            int iNum2 = Int32.Parse(inputNum2);
            // int ทำให้เราสามารถ + - * / ได้
            int iResult = iNum1 / iNum2;
            // ที่ตัวแปรชื่อ result
            // มีคุณสมบัติชื่อ Text
            result.Text = iResult.ToString(); // .ToString = แปรค่าเป็น str
        }

        private void button5_Click(object sender, EventArgs e)
        {
            // ล้างข้อวามในช่อง num1 num2 result
            num1.Text = "";
            num2.Text = "";
            result.Text = "";

        }
    }
}