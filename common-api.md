<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [EcoSaaSCommon API](#ecosaascommon-api)
  - [概览](#%E6%A6%82%E8%A7%88)
    - [版本信息](#%E7%89%88%E6%9C%AC%E4%BF%A1%E6%81%AF)
    - [URI scheme](#uri-scheme)
    - [标签](#%E6%A0%87%E7%AD%BE)
  - [资源](#%E8%B5%84%E6%BA%90)
    - [Email-resource](#email-resource)
      - [发送邮件](#%E5%8F%91%E9%80%81%E9%82%AE%E4%BB%B6)
        - [参数](#%E5%8F%82%E6%95%B0)
        - [响应](#%E5%93%8D%E5%BA%94)
        - [消耗](#%E6%B6%88%E8%80%97)
        - [生成](#%E7%94%9F%E6%88%90)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path)
          - [请求 body](#%E8%AF%B7%E6%B1%82-body)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B)
          - [响应 200](#%E5%93%8D%E5%BA%94-200)
      - [发送带附件的邮件](#%E5%8F%91%E9%80%81%E5%B8%A6%E9%99%84%E4%BB%B6%E7%9A%84%E9%82%AE%E4%BB%B6)
        - [参数](#%E5%8F%82%E6%95%B0-1)
        - [响应](#%E5%93%8D%E5%BA%94-1)
        - [消耗](#%E6%B6%88%E8%80%97-1)
        - [生成](#%E7%94%9F%E6%88%90-1)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-1)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-1)
          - [请求 formData](#%E8%AF%B7%E6%B1%82-formdata)
          - [请求 body](#%E8%AF%B7%E6%B1%82-body-1)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-1)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-1)
    - [Object-resource](#object-resource)
      - [上传文件](#%E4%B8%8A%E4%BC%A0%E6%96%87%E4%BB%B6)
        - [参数](#%E5%8F%82%E6%95%B0-2)
        - [响应](#%E5%93%8D%E5%BA%94-2)
        - [消耗](#%E6%B6%88%E8%80%97-2)
        - [生成](#%E7%94%9F%E6%88%90-2)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-2)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-2)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header)
          - [请求 query](#%E8%AF%B7%E6%B1%82-query)
          - [请求 formData](#%E8%AF%B7%E6%B1%82-formdata-1)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-2)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-2)
      - [获取文件列表](#%E8%8E%B7%E5%8F%96%E6%96%87%E4%BB%B6%E5%88%97%E8%A1%A8)
        - [参数](#%E5%8F%82%E6%95%B0-3)
        - [响应](#%E5%93%8D%E5%BA%94-3)
        - [生成](#%E7%94%9F%E6%88%90-3)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-3)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-3)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-1)
          - [请求 query](#%E8%AF%B7%E6%B1%82-query-1)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-3)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-3)
      - [获取对象的URL的post方法，给后台使用](#%E8%8E%B7%E5%8F%96%E5%AF%B9%E8%B1%A1%E7%9A%84url%E7%9A%84post%E6%96%B9%E6%B3%95%E7%BB%99%E5%90%8E%E5%8F%B0%E4%BD%BF%E7%94%A8)
        - [参数](#%E5%8F%82%E6%95%B0-4)
        - [响应](#%E5%93%8D%E5%BA%94-4)
        - [消耗](#%E6%B6%88%E8%80%97-3)
        - [生成](#%E7%94%9F%E6%88%90-4)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-4)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-4)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-2)
          - [请求 query](#%E8%AF%B7%E6%B1%82-query-2)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-4)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-4)
      - [获取单个文件的信息](#%E8%8E%B7%E5%8F%96%E5%8D%95%E4%B8%AA%E6%96%87%E4%BB%B6%E7%9A%84%E4%BF%A1%E6%81%AF)
        - [参数](#%E5%8F%82%E6%95%B0-5)
        - [响应](#%E5%93%8D%E5%BA%94-5)
        - [生成](#%E7%94%9F%E6%88%90-5)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-5)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-5)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-3)
          - [请求 query](#%E8%AF%B7%E6%B1%82-query-3)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-5)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-5)
      - [删除文件](#%E5%88%A0%E9%99%A4%E6%96%87%E4%BB%B6)
        - [参数](#%E5%8F%82%E6%95%B0-6)
        - [响应](#%E5%93%8D%E5%BA%94-6)
        - [生成](#%E7%94%9F%E6%88%90-6)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-6)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-6)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-4)
          - [请求 query](#%E8%AF%B7%E6%B1%82-query-4)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-6)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-6)
      - [下载文件](#%E4%B8%8B%E8%BD%BD%E6%96%87%E4%BB%B6)
        - [参数](#%E5%8F%82%E6%95%B0-7)
        - [响应](#%E5%93%8D%E5%BA%94-7)
        - [生成](#%E7%94%9F%E6%88%90-7)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-7)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-7)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-5)
          - [请求 query](#%E8%AF%B7%E6%B1%82-query-5)
      - [文件元信息带字节](#%E6%96%87%E4%BB%B6%E5%85%83%E4%BF%A1%E6%81%AF%E5%B8%A6%E5%AD%97%E8%8A%82)
        - [参数](#%E5%8F%82%E6%95%B0-8)
        - [响应](#%E5%93%8D%E5%BA%94-8)
        - [生成](#%E7%94%9F%E6%88%90-8)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-8)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-8)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-6)
          - [请求 query](#%E8%AF%B7%E6%B1%82-query-6)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-7)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-7)
      - [获取对象的URL](#%E8%8E%B7%E5%8F%96%E5%AF%B9%E8%B1%A1%E7%9A%84url)
        - [参数](#%E5%8F%82%E6%95%B0-9)
        - [响应](#%E5%93%8D%E5%BA%94-9)
        - [生成](#%E7%94%9F%E6%88%90-9)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-9)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-9)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-7)
          - [请求 query](#%E8%AF%B7%E6%B1%82-query-7)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-8)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-8)
    - [Ocr](#ocr)
      - [身份证识别，base64图片](#%E8%BA%AB%E4%BB%BD%E8%AF%81%E8%AF%86%E5%88%ABbase64%E5%9B%BE%E7%89%87)
        - [参数](#%E5%8F%82%E6%95%B0-10)
        - [响应](#%E5%93%8D%E5%BA%94-10)
        - [消耗](#%E6%B6%88%E8%80%97-4)
        - [生成](#%E7%94%9F%E6%88%90-10)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-10)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-10)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-8)
          - [请求 query](#%E8%AF%B7%E6%B1%82-query-8)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-9)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-9)
      - [身份证识别，上传文件](#%E8%BA%AB%E4%BB%BD%E8%AF%81%E8%AF%86%E5%88%AB%E4%B8%8A%E4%BC%A0%E6%96%87%E4%BB%B6)
        - [参数](#%E5%8F%82%E6%95%B0-11)
        - [响应](#%E5%93%8D%E5%BA%94-11)
        - [消耗](#%E6%B6%88%E8%80%97-5)
        - [生成](#%E7%94%9F%E6%88%90-11)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-11)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-11)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-9)
          - [请求 query](#%E8%AF%B7%E6%B1%82-query-9)
          - [请求 formData](#%E8%AF%B7%E6%B1%82-formdata-2)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-10)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-10)
    - [Outer-tenant-feign-service](#outer-tenant-feign-service)
      - [findTenantExtend](#findtenantextend)
        - [参数](#%E5%8F%82%E6%95%B0-12)
        - [响应](#%E5%93%8D%E5%BA%94-12)
        - [生成](#%E7%94%9F%E6%88%90-12)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-12)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-12)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-11)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-11)
    - [Sms-resource](#sms-resource)
      - [发送短信](#%E5%8F%91%E9%80%81%E7%9F%AD%E4%BF%A1)
        - [参数](#%E5%8F%82%E6%95%B0-13)
        - [响应](#%E5%93%8D%E5%BA%94-13)
        - [消耗](#%E6%B6%88%E8%80%97-6)
        - [生成](#%E7%94%9F%E6%88%90-13)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-13)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-13)
          - [请求 body](#%E8%AF%B7%E6%B1%82-body-2)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-12)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-12)
    - [Template-resource](#template-resource)
      - [模板查询](#%E6%A8%A1%E6%9D%BF%E6%9F%A5%E8%AF%A2)
        - [参数](#%E5%8F%82%E6%95%B0-14)
        - [响应](#%E5%93%8D%E5%BA%94-14)
        - [生成](#%E7%94%9F%E6%88%90-14)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-14)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-14)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-10)
          - [请求 query](#%E8%AF%B7%E6%B1%82-query-10)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-13)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-13)
      - [新增Email模板](#%E6%96%B0%E5%A2%9Eemail%E6%A8%A1%E6%9D%BF)
        - [参数](#%E5%8F%82%E6%95%B0-15)
        - [响应](#%E5%93%8D%E5%BA%94-15)
        - [消耗](#%E6%B6%88%E8%80%97-7)
        - [生成](#%E7%94%9F%E6%88%90-15)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-15)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-15)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-11)
          - [请求 body](#%E8%AF%B7%E6%B1%82-body-3)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-14)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-14)
      - [获取Email模板](#%E8%8E%B7%E5%8F%96email%E6%A8%A1%E6%9D%BF)
        - [参数](#%E5%8F%82%E6%95%B0-16)
        - [响应](#%E5%93%8D%E5%BA%94-16)
        - [生成](#%E7%94%9F%E6%88%90-16)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-16)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-16)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-12)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-15)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-15)
      - [修改Email模板](#%E4%BF%AE%E6%94%B9email%E6%A8%A1%E6%9D%BF)
        - [参数](#%E5%8F%82%E6%95%B0-17)
        - [响应](#%E5%93%8D%E5%BA%94-17)
        - [消耗](#%E6%B6%88%E8%80%97-8)
        - [生成](#%E7%94%9F%E6%88%90-17)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-17)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-17)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-13)
          - [请求 body](#%E8%AF%B7%E6%B1%82-body-4)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-16)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-16)
      - [删除Email模板](#%E5%88%A0%E9%99%A4email%E6%A8%A1%E6%9D%BF)
        - [参数](#%E5%8F%82%E6%95%B0-18)
        - [响应](#%E5%93%8D%E5%BA%94-18)
        - [生成](#%E7%94%9F%E6%88%90-18)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-18)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-18)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-14)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-17)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-17)
      - [新增SMS模板](#%E6%96%B0%E5%A2%9Esms%E6%A8%A1%E6%9D%BF)
        - [参数](#%E5%8F%82%E6%95%B0-19)
        - [响应](#%E5%93%8D%E5%BA%94-19)
        - [消耗](#%E6%B6%88%E8%80%97-9)
        - [生成](#%E7%94%9F%E6%88%90-19)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-19)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-19)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-15)
          - [请求 body](#%E8%AF%B7%E6%B1%82-body-5)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-18)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-18)
      - [获取SMS模板](#%E8%8E%B7%E5%8F%96sms%E6%A8%A1%E6%9D%BF)
        - [参数](#%E5%8F%82%E6%95%B0-20)
        - [响应](#%E5%93%8D%E5%BA%94-20)
        - [生成](#%E7%94%9F%E6%88%90-20)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-20)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-20)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-16)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-19)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-19)
      - [修改SMS模板](#%E4%BF%AE%E6%94%B9sms%E6%A8%A1%E6%9D%BF)
        - [参数](#%E5%8F%82%E6%95%B0-21)
        - [响应](#%E5%93%8D%E5%BA%94-21)
        - [消耗](#%E6%B6%88%E8%80%97-10)
        - [生成](#%E7%94%9F%E6%88%90-21)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-21)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-21)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-17)
          - [请求 body](#%E8%AF%B7%E6%B1%82-body-6)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-20)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-20)
      - [删除SMS模板](#%E5%88%A0%E9%99%A4sms%E6%A8%A1%E6%9D%BF)
        - [参数](#%E5%8F%82%E6%95%B0-22)
        - [响应](#%E5%93%8D%E5%BA%94-22)
        - [生成](#%E7%94%9F%E6%88%90-22)
        - [HTTP请求示例](#http%E8%AF%B7%E6%B1%82%E7%A4%BA%E4%BE%8B-22)
          - [请求 path](#%E8%AF%B7%E6%B1%82-path-22)
          - [请求 header](#%E8%AF%B7%E6%B1%82-header-18)
        - [HTTP响应示例](#http%E5%93%8D%E5%BA%94%E7%A4%BA%E4%BE%8B-21)
          - [响应 200](#%E5%93%8D%E5%BA%94-200-21)
  - [定义](#%E5%AE%9A%E4%B9%89)
    - [EmailCreateForm](#emailcreateform)
    - [FileMetaWithStreamVO](#filemetawithstreamvo)
    - [FileMetadata](#filemetadata)
    - [PageOfFileMetadata](#pageoffilemetadata)
    - [PageOfTemplate](#pageoftemplate)
    - [RestResponseOfFileMetaWithStreamVO](#restresponseoffilemetawithstreamvo)
    - [RestResponseOfFileMetadata](#restresponseoffilemetadata)
    - [RestResponseOfPageOfFileMetadata](#restresponseofpageoffilemetadata)
    - [RestResponseOfPageOfTemplate](#restresponseofpageoftemplate)
    - [RestResponseOfTemplate](#restresponseoftemplate)
    - [RestResponseOfTenantExtend](#restresponseoftenantextend)
    - [RestResponseOfobject](#restresponseofobject)
    - [RestResponseOfstring](#restresponseofstring)
    - [SmsCreateForm](#smscreateform)
    - [Sort](#sort)
    - [StatusType](#statustype)
    - [Template](#template)
    - [TemplateCreateForm](#templatecreateform)
    - [TemplateUpdateForm](#templateupdateform)
    - [TenantExtend](#tenantextend)
    - [URI](#uri)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# EcoSaaSCommon API


<a name="overview"></a>
## 概览
EcoSaaSCommon API documentation


### 版本信息
*版本* : 0.0.1


### URI scheme
*域名* : ecosaas的域名 //TODO  
*基础路径* : /ecosaascommon


### 标签

* email-resource : 邮件服务
* object-resource : 对象存储
* ocr : 阿里云ocr服务
* outer-tenant-feign-service : Outer Tenant Feign Service
* sms-resource : SMS服务
* template-resource : 模板管理




<a name="paths"></a>
## 资源

<a name="email-resource_resource"></a>
### Email-resource
邮件服务


<a name="sendsingleusingpost"></a>
#### 发送邮件
```
POST /api/ecosaas/common/email/send
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Body**|**emailCreateForm**  <br>*必填*|emailCreateForm|[EmailCreateForm](#emailcreateform)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfstring](#restresponseofstring)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/email/send
```


###### 请求 body
```
json :
{
  "content" : "string",
  "subject" : "string",
  "to" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : "string",
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="sendattachusingpost"></a>
#### 发送带附件的邮件
```
POST /api/ecosaas/common/email/sendAttach
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**FormData**|**file**  <br>*必填*|file|file|
|**Body**|**emailCreateForm**  <br>*必填*|emailCreateForm|[EmailCreateForm](#emailcreateform)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfstring](#restresponseofstring)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `multipart/form-data`


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/email/sendAttach
```


###### 请求 formData
```
json :
"file"
```


###### 请求 body
```
json :
{
  "content" : "string",
  "subject" : "string",
  "to" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : "string",
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="object-resource_resource"></a>
### Object-resource
对象存储


<a name="saveusingpost"></a>
#### 上传文件
```
POST /api/ecosaas/common/oss/object
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Query**|**TenantId**  <br>*必填*|TenantId|string|
|**Query**|**bucketName**  <br>*必填*|bucketName|string|
|**Query**|**filePath**  <br>*可选*|文件保存的路径，不包含文件名|string|
|**FormData**|**file**  <br>*必填*|file|file|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfFileMetadata](#restresponseoffilemetadata)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `multipart/form-data`


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/oss/object
```


###### 请求 header
```
json :
"string"
```


###### 请求 query
```
json :
{
  "TenantId" : "string",
  "bucketName" : "string",
  "filePath" : "string"
}
```


###### 请求 formData
```
json :
"file"
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : {
    "bucketName" : "string",
    "createdBy" : "string",
    "createdDate" : "string",
    "fileName" : "string",
    "fileSize" : 0,
    "fileType" : "string",
    "id" : "string",
    "lastModifiedBy" : "string",
    "lastModifiedDate" : "string",
    "ossId" : "string",
    "path" : "string",
    "storage" : "string"
  },
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="filelistusingget"></a>
#### 获取文件列表
```
GET /api/ecosaas/common/oss/object
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Query**|**TenantId**  <br>*必填*|TenantId|string|
|**Query**|**bucketName**  <br>*可选*||string|
|**Query**|**fileName**  <br>*可选*||string|
|**Query**|**fileSize**  <br>*可选*||integer (int32)|
|**Query**|**fileType**  <br>*可选*||string|
|**Query**|**page**  <br>*可选*|Page number of the requested page|integer (int32)|
|**Query**|**path**  <br>*可选*||string|
|**Query**|**size**  <br>*可选*|Size of a page|integer (int32)|
|**Query**|**sort**  <br>*可选*|Sorting criteria in the format: property(,asc\|desc). Default sort order is ascending. Multiple sort criteria are supported.|< string > array(multi)|
|**Query**|**storage**  <br>*可选*||enum (OSS, NAS)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfPageOfFileMetadata](#restresponseofpageoffilemetadata)|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/oss/object
```


###### 请求 header
```
json :
"string"
```


###### 请求 query
```
json :
{
  "TenantId" : "string",
  "bucketName" : "string",
  "fileName" : "string",
  "fileSize" : 0,
  "fileType" : "string",
  "page" : 0,
  "path" : "string",
  "size" : 0,
  "sort" : "string",
  "storage" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : {
    "content" : [ {
      "bucketName" : "string",
      "createdBy" : "string",
      "createdDate" : "string",
      "fileName" : "string",
      "fileSize" : 0,
      "fileType" : "string",
      "id" : "string",
      "lastModifiedBy" : "string",
      "lastModifiedDate" : "string",
      "ossId" : "string",
      "path" : "string",
      "storage" : "string"
    } ],
    "first" : true,
    "last" : true,
    "number" : 0,
    "numberOfElements" : 0,
    "size" : 0,
    "sort" : { },
    "totalElements" : 0,
    "totalPages" : 0
  },
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="geturlusingpost"></a>
#### 获取对象的URL的post方法，给后台使用
```
POST /api/ecosaas/common/oss/object/url
```


##### 参数

|类型|名称|说明|类型|默认值|
|---|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string||
|**Query**|**TenantId**  <br>*必填*|TenantId|string||
|**Query**|**bucketName**  <br>*必填*|bucketName|string||
|**Query**|**expireMinutes**  <br>*可选*|expireMinutes|integer (int64)|`3600`|
|**Query**|**ossId**  <br>*必填*|ossId|string||


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfstring](#restresponseofstring)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/oss/object/url
```


###### 请求 header
```
json :
"string"
```


###### 请求 query
```
json :
{
  "TenantId" : "string",
  "bucketName" : "string",
  "expireMinutes" : 0,
  "ossId" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : "string",
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="objectinfousingget"></a>
#### 获取单个文件的信息
```
GET /api/ecosaas/common/oss/object/{id}
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Path**|**id**  <br>*必填*|id|string|
|**Query**|**TenantId**  <br>*必填*|TenantId|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfFileMetadata](#restresponseoffilemetadata)|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 生成

* `application/json`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/oss/object/string
```


###### 请求 header
```
json :
"string"
```


###### 请求 query
```
json :
{
  "TenantId" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : {
    "bucketName" : "string",
    "createdBy" : "string",
    "createdDate" : "string",
    "fileName" : "string",
    "fileSize" : 0,
    "fileType" : "string",
    "id" : "string",
    "lastModifiedBy" : "string",
    "lastModifiedDate" : "string",
    "ossId" : "string",
    "path" : "string",
    "storage" : "string"
  },
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="deleteusingdelete"></a>
#### 删除文件
```
DELETE /api/ecosaas/common/oss/object/{id}
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Path**|**id**  <br>*必填*|id|string|
|**Query**|**TenantId**  <br>*必填*|TenantId|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfstring](#restresponseofstring)|
|**204**|No Content|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/oss/object/string
```


###### 请求 header
```
json :
"string"
```


###### 请求 query
```
json :
{
  "TenantId" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : "string",
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="downloadusingget"></a>
#### 下载文件
```
GET /api/ecosaas/common/oss/object/{id}/download
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Path**|**id**  <br>*必填*|id|string|
|**Query**|**TenantId**  <br>*必填*|TenantId|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/oss/object/string/download
```


###### 请求 header
```
json :
"string"
```


###### 请求 query
```
json :
{
  "TenantId" : "string"
}
```


<a name="streamusingget"></a>
#### 文件元信息带字节
```
GET /api/ecosaas/common/oss/object/{id}/stream
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Path**|**id**  <br>*必填*|id|string|
|**Query**|**TenantId**  <br>*必填*|TenantId|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfFileMetaWithStreamVO](#restresponseoffilemetawithstreamvo)|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/oss/object/string/stream
```


###### 请求 header
```
json :
"string"
```


###### 请求 query
```
json :
{
  "TenantId" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : {
    "bucketName" : "string",
    "fileByte" : "string",
    "fileName" : "string",
    "fileSize" : 0,
    "fileType" : "string",
    "ossId" : "string",
    "path" : "string"
  },
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="downloadlinkusingget"></a>
#### 获取对象的URL
```
GET /api/ecosaas/common/oss/object/{id}/url
```


##### 参数

|类型|名称|说明|类型|默认值|
|---|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string||
|**Path**|**id**  <br>*必填*|id|string||
|**Query**|**TenantId**  <br>*必填*|TenantId|string||
|**Query**|**expireMinutes**  <br>*可选*|expireMinutes|integer (int64)|`3600`|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfstring](#restresponseofstring)|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/oss/object/string/url
```


###### 请求 header
```
json :
"string"
```


###### 请求 query
```
json :
{
  "TenantId" : "string",
  "expireMinutes" : 0
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : "string",
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="ocr_resource"></a>
### Ocr
阿里云ocr服务


<a name="idcardbase64identityusingpost"></a>
#### 身份证识别，base64图片
```
POST /api/ecosaas/common/ocr/base64IdCard
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|jwt凭证|string|
|**Query**|**file**  <br>*必填*|身份证文件|string|
|**Query**|**idCardType**  <br>*必填*|身份证的正面还是反面|enum (FACE, BACK)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfstring](#restresponseofstring)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `application/json`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/ocr/base64IdCard
```


###### 请求 header
```
json :
"string"
```


###### 请求 query
```
json :
{
  "file" : "string",
  "idCardType" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : "string",
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="idcardfileidentityusingpost"></a>
#### 身份证识别，上传文件
```
POST /api/ecosaas/common/ocr/idCard
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|jwt凭证|string|
|**Query**|**idCardType**  <br>*必填*|身份证的正面还是反面|enum (FACE, BACK)|
|**FormData**|**file**  <br>*必填*|身份证文件|file|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfstring](#restresponseofstring)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `multipart/form-data`


##### 生成

* `application/json`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/ocr/idCard
```


###### 请求 header
```
json :
"string"
```


###### 请求 query
```
json :
{
  "idCardType" : "string"
}
```


###### 请求 formData
```
json :
"file"
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : "string",
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="outer-tenant-feign-service_resource"></a>
### Outer-tenant-feign-service
Outer Tenant Feign Service


<a name="findtenantextendusingget"></a>
#### findTenantExtend
```
GET /api/ecosaas/store/tenant/sso/extend/{tenantId}/key/{extendKey}
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Path**|**extendKey**  <br>*必填*|extendKey|string|
|**Path**|**tenantId**  <br>*必填*|tenantId|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfTenantExtend](#restresponseoftenantextend)|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/store/tenant/sso/extend/string/key/string
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : {
    "createdBy" : "string",
    "createdDate" : "string",
    "extendKey" : "string",
    "extendValue" : "string",
    "id" : "string",
    "lastModifiedBy" : "string",
    "lastModifiedDate" : "string",
    "tenantId" : "string"
  },
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="sms-resource_resource"></a>
### Sms-resource
SMS服务


<a name="sendusingpost"></a>
#### 发送短信
```
POST /api/ecosaas/common/sms/send
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Body**|**smsCreateForm**  <br>*必填*|smsCreateForm|[SmsCreateForm](#smscreateform)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfstring](#restresponseofstring)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `application/json`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/sms/send
```


###### 请求 body
```
json :
{
  "code" : "string",
  "map" : {
    "string" : "string"
  },
  "mobile" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : "string",
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="template-resource_resource"></a>
### Template-resource
模板管理


<a name="listtemplatesusingget"></a>
#### 模板查询
```
GET /api/ecosaas/common/template/
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Query**|**context**  <br>*可选*||string|
|**Query**|**langCode**  <br>*可选*||string|
|**Query**|**page**  <br>*可选*|Page number of the requested page|integer (int32)|
|**Query**|**size**  <br>*可选*|Size of a page|integer (int32)|
|**Query**|**sort**  <br>*可选*|Sorting criteria in the format: property(,asc\|desc). Default sort order is ascending. Multiple sort criteria are supported.|< string > array(multi)|
|**Query**|**subject**  <br>*可选*||string|
|**Query**|**templateType**  <br>*可选*||enum (EMAIL, SMS)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfPageOfTemplate](#restresponseofpageoftemplate)|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 生成

* `application/json`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/template/
```


###### 请求 header
```
json :
"string"
```


###### 请求 query
```
json :
{
  "context" : "string",
  "langCode" : "string",
  "page" : 0,
  "size" : 0,
  "sort" : "string",
  "subject" : "string",
  "templateType" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : {
    "content" : [ {
      "businessCode" : "string",
      "code" : "string",
      "context" : "string",
      "createdBy" : "string",
      "createdDate" : "string",
      "id" : "string",
      "langCode" : "string",
      "lastModifiedBy" : "string",
      "lastModifiedDate" : "string",
      "subject" : "string",
      "templateType" : "string"
    } ],
    "first" : true,
    "last" : true,
    "number" : 0,
    "numberOfElements" : 0,
    "size" : 0,
    "sort" : { },
    "totalElements" : 0,
    "totalPages" : 0
  },
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="saveemailusingpost"></a>
#### 新增Email模板
```
POST /api/ecosaas/common/template/email
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Body**|**templateCreateForm**  <br>*必填*|templateCreateForm|[TemplateCreateForm](#templatecreateform)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfTemplate](#restresponseoftemplate)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `application/json`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/template/email
```


###### 请求 header
```
json :
"string"
```


###### 请求 body
```
json :
{
  "businessCode" : "string",
  "code" : "string",
  "context" : "string",
  "langCode" : "string",
  "subject" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : {
    "businessCode" : "string",
    "code" : "string",
    "context" : "string",
    "createdBy" : "string",
    "createdDate" : "string",
    "id" : "string",
    "langCode" : "string",
    "lastModifiedBy" : "string",
    "lastModifiedDate" : "string",
    "subject" : "string",
    "templateType" : "string"
  },
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="findoneemailtemplateusingget"></a>
#### 获取Email模板
```
GET /api/ecosaas/common/template/email/{businessCode}
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Path**|**businessCode**  <br>*必填*|businessCode|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfTemplate](#restresponseoftemplate)|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 生成

* `application/json`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/template/email/string
```


###### 请求 header
```
json :
"string"
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : {
    "businessCode" : "string",
    "code" : "string",
    "context" : "string",
    "createdBy" : "string",
    "createdDate" : "string",
    "id" : "string",
    "langCode" : "string",
    "lastModifiedBy" : "string",
    "lastModifiedDate" : "string",
    "subject" : "string",
    "templateType" : "string"
  },
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="updateemailusingput"></a>
#### 修改Email模板
```
PUT /api/ecosaas/common/template/email/{businessCode}
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Path**|**businessCode**  <br>*必填*|businessCode|string|
|**Body**|**templateUpdateForm**  <br>*必填*|templateUpdateForm|[TemplateUpdateForm](#templateupdateform)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfTemplate](#restresponseoftemplate)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `application/json`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/template/email/string
```


###### 请求 header
```
json :
"string"
```


###### 请求 body
```
json :
{
  "businessCode" : "string",
  "code" : "string",
  "context" : "string",
  "langCode" : "string",
  "subject" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : {
    "businessCode" : "string",
    "code" : "string",
    "context" : "string",
    "createdBy" : "string",
    "createdDate" : "string",
    "id" : "string",
    "langCode" : "string",
    "lastModifiedBy" : "string",
    "lastModifiedDate" : "string",
    "subject" : "string",
    "templateType" : "string"
  },
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="deleteoneemailusingdelete"></a>
#### 删除Email模板
```
DELETE /api/ecosaas/common/template/email/{businessCode}
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Path**|**businessCode**  <br>*必填*|businessCode|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfobject](#restresponseofobject)|
|**204**|No Content|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|


##### 生成

* `application/json`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/template/email/string
```


###### 请求 header
```
json :
"string"
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : "object",
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="savesmsusingpost"></a>
#### 新增SMS模板
```
POST /api/ecosaas/common/template/sms
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Body**|**templateCreateForm**  <br>*必填*|templateCreateForm|[TemplateCreateForm](#templatecreateform)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfTemplate](#restresponseoftemplate)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `application/json`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/template/sms
```


###### 请求 header
```
json :
"string"
```


###### 请求 body
```
json :
{
  "businessCode" : "string",
  "code" : "string",
  "context" : "string",
  "langCode" : "string",
  "subject" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : {
    "businessCode" : "string",
    "code" : "string",
    "context" : "string",
    "createdBy" : "string",
    "createdDate" : "string",
    "id" : "string",
    "langCode" : "string",
    "lastModifiedBy" : "string",
    "lastModifiedDate" : "string",
    "subject" : "string",
    "templateType" : "string"
  },
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="findonesmstemplateusingget"></a>
#### 获取SMS模板
```
GET /api/ecosaas/common/template/sms/{businessCode}
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Path**|**businessCode**  <br>*必填*|businessCode|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfTemplate](#restresponseoftemplate)|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 生成

* `application/json`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/template/sms/string
```


###### 请求 header
```
json :
"string"
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : {
    "businessCode" : "string",
    "code" : "string",
    "context" : "string",
    "createdBy" : "string",
    "createdDate" : "string",
    "id" : "string",
    "langCode" : "string",
    "lastModifiedBy" : "string",
    "lastModifiedDate" : "string",
    "subject" : "string",
    "templateType" : "string"
  },
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="updatesmsusingput"></a>
#### 修改SMS模板
```
PUT /api/ecosaas/common/template/sms/{businessCode}
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Path**|**businessCode**  <br>*必填*|businessCode|string|
|**Body**|**templateUpdateForm**  <br>*必填*|templateUpdateForm|[TemplateUpdateForm](#templateupdateform)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfTemplate](#restresponseoftemplate)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `application/json`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/template/sms/string
```


###### 请求 header
```
json :
"string"
```


###### 请求 body
```
json :
{
  "businessCode" : "string",
  "code" : "string",
  "context" : "string",
  "langCode" : "string",
  "subject" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : {
    "businessCode" : "string",
    "code" : "string",
    "context" : "string",
    "createdBy" : "string",
    "createdDate" : "string",
    "id" : "string",
    "langCode" : "string",
    "lastModifiedBy" : "string",
    "lastModifiedDate" : "string",
    "subject" : "string",
    "templateType" : "string"
  },
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```


<a name="deleteonesmsusingdelete"></a>
#### 删除SMS模板
```
DELETE /api/ecosaas/common/template/sms/{businessCode}
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**Authorization**  <br>*必填*|Authorization|string|
|**Path**|**businessCode**  <br>*必填*|businessCode|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[RestResponseOfobject](#restresponseofobject)|
|**204**|No Content|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|


##### 生成

* `application/json`


##### HTTP请求示例

###### 请求 path
```
/api/ecosaas/common/template/sms/string
```


###### 请求 header
```
json :
"string"
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "bizCode" : "string",
  "data" : "object",
  "detail" : "string",
  "instance" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  },
  "message" : "string",
  "status" : {
    "reasonPhrase" : "string",
    "statusCode" : 0
  },
  "title" : "string",
  "type" : {
    "absolute" : true,
    "authority" : "string",
    "fragment" : "string",
    "host" : "string",
    "opaque" : true,
    "path" : "string",
    "port" : 0,
    "query" : "string",
    "rawAuthority" : "string",
    "rawFragment" : "string",
    "rawPath" : "string",
    "rawQuery" : "string",
    "rawSchemeSpecificPart" : "string",
    "rawUserInfo" : "string",
    "scheme" : "string",
    "schemeSpecificPart" : "string",
    "userInfo" : "string"
  }
}
```




<a name="definitions"></a>
## 定义

<a name="emailcreateform"></a>
### EmailCreateForm

|名称|说明|类型|
|---|---|---|
|**content**  <br>*可选*|**样例** : `"string"`|string|
|**subject**  <br>*可选*|**样例** : `"string"`|string|
|**to**  <br>*可选*|**样例** : `"string"`|string|


<a name="filemetawithstreamvo"></a>
### FileMetaWithStreamVO

|名称|说明|类型|
|---|---|---|
|**bucketName**  <br>*可选*|**样例** : `"string"`|string|
|**fileByte**  <br>*可选*|**模式** : `"^(?:[A-Za-z0-9+/]{4})*(?:[A-Za-z0-9+/]{2}==\|[A-Za-z0-9+/]{3}=)?$"`**样例** : `"string"`|string (byte)|
|**fileName**  <br>*可选*|**样例** : `"string"`|string|
|**fileSize**  <br>*可选*|**样例** : `0`|integer (int32)|
|**fileType**  <br>*可选*|**样例** : `"string"`|string|
|**ossId**  <br>*可选*|**样例** : `"string"`|string|
|**path**  <br>*可选*|**样例** : `"string"`|string|


<a name="filemetadata"></a>
### FileMetadata

|名称|说明|类型|
|---|---|---|
|**bucketName**  <br>*可选*|**样例** : `"string"`|string|
|**createdBy**  <br>*可选*|**样例** : `"string"`|string|
|**createdDate**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**fileName**  <br>*可选*|**样例** : `"string"`|string|
|**fileSize**  <br>*可选*|**样例** : `0`|integer (int32)|
|**fileType**  <br>*可选*|**样例** : `"string"`|string|
|**id**  <br>*可选*|**样例** : `"string"`|string|
|**lastModifiedBy**  <br>*可选*|**样例** : `"string"`|string|
|**lastModifiedDate**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**ossId**  <br>*可选*|**样例** : `"string"`|string|
|**path**  <br>*可选*|**样例** : `"string"`|string|
|**storage**  <br>*可选*|**样例** : `"string"`|enum (OSS, NAS)|


<a name="pageoffilemetadata"></a>
### PageOfFileMetadata

|名称|说明|类型|
|---|---|---|
|**content**  <br>*可选*|**样例** : `[ "[filemetadata](#filemetadata)" ]`|< [FileMetadata](#filemetadata) > array|
|**first**  <br>*可选*|**样例** : `true`|boolean|
|**last**  <br>*可选*|**样例** : `true`|boolean|
|**number**  <br>*可选*|**样例** : `0`|integer (int32)|
|**numberOfElements**  <br>*可选*|**样例** : `0`|integer (int32)|
|**size**  <br>*可选*|**样例** : `0`|integer (int32)|
|**sort**  <br>*可选*|**样例** : `"[sort](#sort)"`|[Sort](#sort)|
|**totalElements**  <br>*可选*|**样例** : `0`|integer (int64)|
|**totalPages**  <br>*可选*|**样例** : `0`|integer (int32)|


<a name="pageoftemplate"></a>
### PageOfTemplate

|名称|说明|类型|
|---|---|---|
|**content**  <br>*可选*|**样例** : `[ "[template](#template)" ]`|< [Template](#template) > array|
|**first**  <br>*可选*|**样例** : `true`|boolean|
|**last**  <br>*可选*|**样例** : `true`|boolean|
|**number**  <br>*可选*|**样例** : `0`|integer (int32)|
|**numberOfElements**  <br>*可选*|**样例** : `0`|integer (int32)|
|**size**  <br>*可选*|**样例** : `0`|integer (int32)|
|**sort**  <br>*可选*|**样例** : `"[sort](#sort)"`|[Sort](#sort)|
|**totalElements**  <br>*可选*|**样例** : `0`|integer (int64)|
|**totalPages**  <br>*可选*|**样例** : `0`|integer (int32)|


<a name="restresponseoffilemetawithstreamvo"></a>
### RestResponseOfFileMetaWithStreamVO

|名称|说明|类型|
|---|---|---|
|**bizCode**  <br>*可选*|**样例** : `"string"`|string|
|**data**  <br>*可选*|**样例** : `"[filemetawithstreamvo](#filemetawithstreamvo)"`|[FileMetaWithStreamVO](#filemetawithstreamvo)|
|**detail**  <br>*可选*|**样例** : `"string"`|string|
|**instance**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|
|**message**  <br>*可选*|**样例** : `"string"`|string|
|**status**  <br>*可选*|**样例** : `"[statustype](#statustype)"`|[StatusType](#statustype)|
|**title**  <br>*可选*|**样例** : `"string"`|string|
|**type**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|


<a name="restresponseoffilemetadata"></a>
### RestResponseOfFileMetadata

|名称|说明|类型|
|---|---|---|
|**bizCode**  <br>*可选*|**样例** : `"string"`|string|
|**data**  <br>*可选*|**样例** : `"[filemetadata](#filemetadata)"`|[FileMetadata](#filemetadata)|
|**detail**  <br>*可选*|**样例** : `"string"`|string|
|**instance**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|
|**message**  <br>*可选*|**样例** : `"string"`|string|
|**status**  <br>*可选*|**样例** : `"[statustype](#statustype)"`|[StatusType](#statustype)|
|**title**  <br>*可选*|**样例** : `"string"`|string|
|**type**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|


<a name="restresponseofpageoffilemetadata"></a>
### RestResponseOfPageOfFileMetadata

|名称|说明|类型|
|---|---|---|
|**bizCode**  <br>*可选*|**样例** : `"string"`|string|
|**data**  <br>*可选*|**样例** : `"[pageoffilemetadata](#pageoffilemetadata)"`|[PageOfFileMetadata](#pageoffilemetadata)|
|**detail**  <br>*可选*|**样例** : `"string"`|string|
|**instance**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|
|**message**  <br>*可选*|**样例** : `"string"`|string|
|**status**  <br>*可选*|**样例** : `"[statustype](#statustype)"`|[StatusType](#statustype)|
|**title**  <br>*可选*|**样例** : `"string"`|string|
|**type**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|


<a name="restresponseofpageoftemplate"></a>
### RestResponseOfPageOfTemplate

|名称|说明|类型|
|---|---|---|
|**bizCode**  <br>*可选*|**样例** : `"string"`|string|
|**data**  <br>*可选*|**样例** : `"[pageoftemplate](#pageoftemplate)"`|[PageOfTemplate](#pageoftemplate)|
|**detail**  <br>*可选*|**样例** : `"string"`|string|
|**instance**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|
|**message**  <br>*可选*|**样例** : `"string"`|string|
|**status**  <br>*可选*|**样例** : `"[statustype](#statustype)"`|[StatusType](#statustype)|
|**title**  <br>*可选*|**样例** : `"string"`|string|
|**type**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|


<a name="restresponseoftemplate"></a>
### RestResponseOfTemplate

|名称|说明|类型|
|---|---|---|
|**bizCode**  <br>*可选*|**样例** : `"string"`|string|
|**data**  <br>*可选*|**样例** : `"[template](#template)"`|[Template](#template)|
|**detail**  <br>*可选*|**样例** : `"string"`|string|
|**instance**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|
|**message**  <br>*可选*|**样例** : `"string"`|string|
|**status**  <br>*可选*|**样例** : `"[statustype](#statustype)"`|[StatusType](#statustype)|
|**title**  <br>*可选*|**样例** : `"string"`|string|
|**type**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|


<a name="restresponseoftenantextend"></a>
### RestResponseOfTenantExtend

|名称|说明|类型|
|---|---|---|
|**bizCode**  <br>*可选*|**样例** : `"string"`|string|
|**data**  <br>*可选*|**样例** : `"[tenantextend](#tenantextend)"`|[TenantExtend](#tenantextend)|
|**detail**  <br>*可选*|**样例** : `"string"`|string|
|**instance**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|
|**message**  <br>*可选*|**样例** : `"string"`|string|
|**status**  <br>*可选*|**样例** : `"[statustype](#statustype)"`|[StatusType](#statustype)|
|**title**  <br>*可选*|**样例** : `"string"`|string|
|**type**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|


<a name="restresponseofobject"></a>
### RestResponseOfobject

|名称|说明|类型|
|---|---|---|
|**bizCode**  <br>*可选*|**样例** : `"string"`|string|
|**data**  <br>*可选*|**样例** : `"object"`|object|
|**detail**  <br>*可选*|**样例** : `"string"`|string|
|**instance**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|
|**message**  <br>*可选*|**样例** : `"string"`|string|
|**status**  <br>*可选*|**样例** : `"[statustype](#statustype)"`|[StatusType](#statustype)|
|**title**  <br>*可选*|**样例** : `"string"`|string|
|**type**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|


<a name="restresponseofstring"></a>
### RestResponseOfstring

|名称|说明|类型|
|---|---|---|
|**bizCode**  <br>*可选*|**样例** : `"string"`|string|
|**data**  <br>*可选*|**样例** : `"string"`|string|
|**detail**  <br>*可选*|**样例** : `"string"`|string|
|**instance**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|
|**message**  <br>*可选*|**样例** : `"string"`|string|
|**status**  <br>*可选*|**样例** : `"[statustype](#statustype)"`|[StatusType](#statustype)|
|**title**  <br>*可选*|**样例** : `"string"`|string|
|**type**  <br>*可选*|**样例** : `"[uri](#uri)"`|[URI](#uri)|


<a name="smscreateform"></a>
### SmsCreateForm

|名称|说明|类型|
|---|---|---|
|**code**  <br>*可选*|**样例** : `"string"`|string|
|**map**  <br>*可选*|**样例** : `{<br>  "string" : "string"<br>}`|< string, string > map|
|**mobile**  <br>*可选*|**样例** : `"string"`|string|


<a name="sort"></a>
### Sort
*类型* : object


<a name="statustype"></a>
### StatusType

|名称|说明|类型|
|---|---|---|
|**reasonPhrase**  <br>*可选*|**样例** : `"string"`|string|
|**statusCode**  <br>*可选*|**样例** : `0`|integer (int32)|


<a name="template"></a>
### Template

|名称|说明|类型|
|---|---|---|
|**businessCode**  <br>*可选*|**样例** : `"string"`|string|
|**code**  <br>*可选*|**样例** : `"string"`|string|
|**context**  <br>*可选*|**样例** : `"string"`|string|
|**createdBy**  <br>*可选*|**样例** : `"string"`|string|
|**createdDate**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**id**  <br>*可选*|**样例** : `"string"`|string|
|**langCode**  <br>*可选*|**样例** : `"string"`|string|
|**lastModifiedBy**  <br>*可选*|**样例** : `"string"`|string|
|**lastModifiedDate**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**subject**  <br>*可选*|**样例** : `"string"`|string|
|**templateType**  <br>*可选*|**样例** : `"string"`|string|


<a name="templatecreateform"></a>
### TemplateCreateForm

|名称|说明|类型|
|---|---|---|
|**businessCode**  <br>*可选*|**样例** : `"string"`|string|
|**code**  <br>*可选*|**样例** : `"string"`|string|
|**context**  <br>*可选*|**样例** : `"string"`|string|
|**langCode**  <br>*可选*|**样例** : `"string"`|string|
|**subject**  <br>*可选*|**样例** : `"string"`|string|


<a name="templateupdateform"></a>
### TemplateUpdateForm

|名称|说明|类型|
|---|---|---|
|**businessCode**  <br>*可选*|**样例** : `"string"`|string|
|**code**  <br>*可选*|**样例** : `"string"`|string|
|**context**  <br>*可选*|**样例** : `"string"`|string|
|**langCode**  <br>*可选*|**样例** : `"string"`|string|
|**subject**  <br>*可选*|**样例** : `"string"`|string|


<a name="tenantextend"></a>
### TenantExtend

|名称|说明|类型|
|---|---|---|
|**createdBy**  <br>*可选*|**样例** : `"string"`|string|
|**createdDate**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**extendKey**  <br>*可选*|**长度** : `0 - 200`**样例** : `"string"`|string|
|**extendValue**  <br>*可选*|**长度** : `0 - 500`**样例** : `"string"`|string|
|**id**  <br>*可选*|**样例** : `"string"`|string|
|**lastModifiedBy**  <br>*可选*|**样例** : `"string"`|string|
|**lastModifiedDate**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**tenantId**  <br>*可选*|**样例** : `"string"`|string|


<a name="uri"></a>
### URI

|名称|说明|类型|
|---|---|---|
|**absolute**  <br>*可选*|**样例** : `true`|boolean|
|**authority**  <br>*可选*|**样例** : `"string"`|string|
|**fragment**  <br>*可选*|**样例** : `"string"`|string|
|**host**  <br>*可选*|**样例** : `"string"`|string|
|**opaque**  <br>*可选*|**样例** : `true`|boolean|
|**path**  <br>*可选*|**样例** : `"string"`|string|
|**port**  <br>*可选*|**样例** : `0`|integer (int32)|
|**query**  <br>*可选*|**样例** : `"string"`|string|
|**rawAuthority**  <br>*可选*|**样例** : `"string"`|string|
|**rawFragment**  <br>*可选*|**样例** : `"string"`|string|
|**rawPath**  <br>*可选*|**样例** : `"string"`|string|
|**rawQuery**  <br>*可选*|**样例** : `"string"`|string|
|**rawSchemeSpecificPart**  <br>*可选*|**样例** : `"string"`|string|
|**rawUserInfo**  <br>*可选*|**样例** : `"string"`|string|
|**scheme**  <br>*可选*|**样例** : `"string"`|string|
|**schemeSpecificPart**  <br>*可选*|**样例** : `"string"`|string|
|**userInfo**  <br>*可选*|**样例** : `"string"`|string|





