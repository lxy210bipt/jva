# jva
实验报告<br>
=========

实验目的:<br>
1、设计GUI窗体，支持学生注册、课程新加、学生选课、学生退课、打印学生选课列表等操作。<br>
2、基于事件模型对业务逻辑编程，实现在界面上支持上述操作。<br>
3、针对操作过程中可能会出现的各种异常，做异常处理<br>
4、基于输入/输出编程，支持学生、课程、教师等数据的读写操作。<br>
5、基于Github.com提交实验，包括实验SRC源文件夹程序、README.MD实验报告文档。<br>

程序框图<br>
==========

![Image discription](https://github.com/lxy210bipt/jva/blob/master/%E6%9D%8E%E6%97%AD%E6%B4%8B.jpg.PNG)

截图<br>
=========

![Image discription](https://github.com/lxy210bipt/jva/blob/master/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20191208225654.jpg)

核心代码<br>
package GUI;<br>
import java.awt.EventQueue;<br>
import javax.swing.JFrame;<br>
import java.awt.event.ActionListener;<br>
import java.awt.event.ActionEvent;<br>
import javax.swing.JPanel;<br>
import javax.swing.border.EmptyBorder;<br>
import javax.swing.JButton;<br>
public index() {<br>
	setTitle("index");<br>
	setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);<br>
	setBounds(150, 150, 500, 350);<br>
	contentPane = new JPanel();<br>
	contentPane.setBorder(new EmptyBorder(10, 10, 10, 10));<br>
	setContentPane(contentPane);<br>
	contentPane.setLayout(null);<br>
	JButton btnNewButton = new JButton("exit");<br>
	btnNewButton.setBounds(0, 110, 100, 30);<br>
	contentPane.add(btnNewButton);<br>
	btnNewButton.addActionListener(new ActionListener(){<br>
		public void actionPerformed(ActionEvent e) {<br>
			Exit exit = new Exit();<br>
			exit.setVisible(true);<br>
			}<br>
		});<br>
	JButton btnNewButton_1 = new JButton("Chose");<br>
	btnNewButton_1.setBounds(350, 110, 100, 30);<br>
	contentPane.add(btnNewButton_1);<br>
	btnNewButton_1.addActionListener(new ActionListener(){<br>
		public void actionPerformed(ActionEvent e) {<br>
			chose chose = new chose();<br>
			chose.setVisible(true); <br>
			}<br>
		});<br>
	JButton btnNewButton_3 = new JButton("Print");<br>
	contentPane.add(btnNewButton_3);<br>
	btnNewButton_3.setBounds(180, 110, 100, 30);<br>
	btnNewButton_3.addActionListener(new ActionListener(){<br>
		public void actionPerformed(ActionEvent e) {<br>
			Print print = new Print();<br>
			print.setVisible(true);<br>
			}<br>
		});<br>
	}<br>

}<br>

实验感想<br>
==========

通过本次实验我学会了GUI编程设计，其中从建立框架到button的构建，课程信息导入都出现了不同问题，后来通过查阅课本，向同学请教最后得以解决。这个实验不仅培养了我的Java编程逻辑更是提高了独立解决分析问题的能力。
