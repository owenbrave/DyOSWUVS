# weixin452-springboot校园选课小程序

## 前言

本项目是一款基于Spring Boot的校园选课小程序，致力于为高校师生提供便捷、高效的选课服务。通过本小程序，学生可以轻松查看课程信息、选择课程，教师也可以方便地进行课程管理。以下是本项目的详细介绍。

## 内容介绍

本项目主要包括以下功能模块：

1. 课程展示：展示所有可选课程，包括课程名称、教师、上课时间等。
2. 课程搜索：支持按课程名称、教师名称进行搜索。
3. 选课操作：学生可以添加、删除所选课程。
4. 个人中心：查看已选课程，进行课程退选等操作。
5. 教师管理：教师可以发布、修改、删除课程信息。

## 技术介绍

本项目采用以下技术栈：

- 语言：Java
- 使用框架：Spring Boot、Spring MVC、MyBatis、微信小程序
- 前端技术：JS、Vue、CSS3、Uniapp
- 开发工具：IDEA/Eclipse、Uniapp
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven：apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

## 核心代码

以下是本项目中的部分核心代码：

```java
// CourseController.java
@RestController
@RequestMapping("/api/course")
public class CourseController {

    @Autowired
    private CourseService courseService;

    // 查询所有课程
    @GetMapping("/list")
    public ResponseEntity<List<Course>> list() {
        List<Course> courses = courseService.list();
        return ResponseEntity.ok(courses);
    }

    // 添加课程
    @PostMapping("/add")
    public ResponseEntity<Void> add(@RequestBody Course course) {
        courseService.add(course);
        return ResponseEntity.ok().build();
    }
}
```

## 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

## 项目截图
