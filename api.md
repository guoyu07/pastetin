FORMAT: 1A

# YYQB API

# Goods [/api/goods]
产品相关接口

## 获取产品列表 [GET /api/goods]


+ Response 200 (application/json)
    + Body

            {
                "code": 0,
                "msg": "ok",
                "data": [
                    {
                        "name": "u4ea7u54c1u540du79f0",
                        "sku": "123",
                        "slogan": "u8fd0u8425u63a8u5e7fu8bed!",
                        "img_small": "u5c0fu56feu94feu63a5"
                    }
                ]
            }

## 创建一个新的产品 [POST /api/goods]


+ Request (application/json)
    + Body

            {
                "name": "u4ea7u54c1u540du79f0",
                "sku": "123",
                "slogan": "WTF",
                "img_small": "WTF"
            }

+ Response 200 (application/json)
    + Body

            {
                "code": 0,
                "msg": "ok"
            }

## 删除一个产品 [DELETE /api/goods/{id}]


+ Parameters
    + id (string, optional) - 产品id

+ Response 200 (application/json)
    + Body

            {
                "code": 0,
                "msg": "ok"
            }

# AppHttpControllersRoundController

# AppHttpControllersOrderController

# AppHttpControllersLotteryController

# Banners [/api/banners]
Banner相关接口

## 获取banner列表 [GET /api/banners]


+ Response 200 (application/json)
    + Body

            {
                "code": 0,
                "msg": "ok",
                "data": [
                    {
                        "id": 1,
                        "img_src": "www.test.com/test.jpg",
                        "jump_target": "http://www.jump.com",
                        "active": 0,
                        "created_at": 111111,
                        "updated_at": 111111
                    }
                ]
            }

## 创建一个新的banner [POST /api/banners]


+ Request (application/json)
    + Body

            {
                "img_src": "img url here",
                "jump_target": "where to jump?"
            }

+ Response 200 (application/json)
    + Body

            {
                "code": 0,
                "msg": "ok"
            }

## 删除一个banner [DELETE /api/banners/{id}]


+ Parameters
    + id (string, optional) - id of banner

+ Response 200 (application/json)
    + Body

            {
                "code": 0,
                "msg": "ok"
            }
