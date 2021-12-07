实验一 程序组织及验证
实验目的：
基本掌握本人所选择的集成开发工具的使用方法 掌握Java源程序命名、运行方法 理解、掌握创建包的方法 初步了解类的实例化方法
实验要求：
定义包组织类定义类的属性、方法
实验步骤：
一：给出了程序的源文件（如下面的三个源文件），请阅读、理解其功能、含义，分析如下三个Java源程序文件的关系，理解以下三个源文件表达的实体业务逻辑关系（源文件分别描述了银行账户、存款人员、测试类）。 
二：在开发环境中组织代码并运行。 
三：请在Customer类新添加一个属性，描述其年龄，并补充操作年龄的方法。在测试类中调用这些方法。 
四：在理解上述程序的情况下，尝试从头分析并复写该程序
关键代码：
public class TestBanking {

   public static void main(String[] args) {
        Customer customer;
        Account account;
        System.out.println("Creating the customer xuan yin.");
        customer=new Customer("yin","xuan",19);
        System.out.println("Creating hisaccount with a 500.00 balance.");
        customer.setAccount(new Account(500.00));
        account=customer.getAccount();
        System.out.println("Withdraw150.00:"+account.withdraw(150.00));
        System.out.println("Deposit22.50:"+account.deposit(22.50));
        System.out.println("Withdraw47.62:"+account.withdraw(47.62));
        System.out.println("Withdraw400.00:"+account.withdraw(400.00));
        System.out.println("Customer["+customer.getLastName()+","+customer.getFirstName()+","+customer.getage()+"]has abalance of"+account.getBalance());

运行结果截图：
![121307_9ae00ff6_9902646](https://user-images.githubusercontent.com/92964321/144984102-1620dfe2-c6cf-4243-b2fe-5c6088053628.png)
实验感想：
通过本次实验我基本掌握所选择的集成开发工具IDEA的使用方法，掌握了Java源程序命名、运行方法理解、掌握了创建包的方法初步了解类的实例化方法。本次实验让我对代码的理解更加深刻。
