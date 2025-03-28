import React from 'react';
import { Button } from '@/components/ui/button';
import { Card, CardContent } from '@/components/ui/card';
import { motion } from 'framer-motion';

export default function ProductAd() {
  return (
    <div className="min-h-screen bg-gradient-to-br from-blue-500 to-purple-600 flex flex-col items-center justify-center p-4">
      <motion.h1 
        className="text-5xl font-bold text-white mb-4"
        initial={{ opacity: 0, y: -50 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 0.5 }}
      >
        Представляем: Новый Продукт!
      </motion.h1>
      <Card className="w-full max-w-md bg-white shadow-2xl rounded-2xl">
        <CardContent className="p-6 text-center">
          <img 
            src="/product-image.jpg" 
            alt="Product" 
            className="w-full h-64 object-cover rounded-xl mb-4"
          />
          <h2 className="text-2xl font-semibold mb-2">Лучшее решение для вас</h2>
          <p className="text-gray-600 mb-4">
            Откройте новые возможности с нашим инновационным продуктом.
          </p>
          <Button className="bg-blue-500 hover:bg-blue-600 text-white px-4 py-2 rounded-full">
            Узнать больше
          </Button>
        </CardContent>
      </Card>
      <motion.div 
        className="mt-8 text-white text-center"
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        transition={{ delay: 0.5, duration: 0.5 }}
      >
        <p>✨ Не упустите шанс первыми испытать наш продукт!</p>
      </motion.div>
      
      <div className="mt-8 w-full max-w-md bg-white p-6 rounded-2xl shadow-lg">
        <h3 className="text-xl font-semibold mb-4 text-gray-800">Отзывы клиентов</h3>
        <div className="mb-4">
          <p className="text-gray-700">"Этот продукт изменил мою жизнь!" — <strong>Анна</strong></p>
        </div>
        <div className="mb-4">
          <p className="text-gray-700">"Высокое качество и отличный сервис." — <strong>Игорь</strong></p>
        </div>
        <div>
          <p className="text-gray-700">"Рекомендую всем, кто ценит комфорт." — <strong>Ольга</strong></p>
        </div>
      </div>

      <div className="mt-8 w-full max-w-md bg-white p-6 rounded-2xl shadow-lg">
        <h3 className="text-xl font-semibold mb-4 text-gray-800">Свяжитесь с нами</h3>
        <form className="flex flex-col space-y-4">
          <input 
            type="text" 
            placeholder="Ваше имя" 
            className="p-2 border border-gray-300 rounded-lg" 
          />
          <input 
            type="email" 
            placeholder="Ваш email" 
            className="p-2 border border-gray-300 rounded-lg" 
          />
          <textarea 
            placeholder="Ваше сообщение" 
            className="p-2 border border-gray-300 rounded-lg h-32"
          ></textarea>
          <Button className="bg-blue-500 hover:bg-blue-600 text-white px-4 py-2 rounded-full">
            Отправить
          </Button>
        </form>
      </div>
    </div>
  );
}
---
id: documentation-intro
title: About the Documentation
sidebar_label: About Docs
---

Welcome to the Create React App documentation!

## Navigation

You can find different topics in the table of contents. On desktop, you should see it in the left sidebar. On mobile, you should see it after pressing an icon with arrows in the top left corner.

## Looking for React Docs?

The documentation for React itself is located on a separate website: **[reactjs.org](https://reactjs.org/)**.

This website is only about Create React App.

## Something Missing?

If you have ideas for more “How To” recipes that should be on this page, [let us know](https://github.com/facebook/create-react-app/issues) or [contribute some!](https://github.com/facebook/create-react-app/tree/main/docusaurus/docs)

## Feedback

We are always open to [your feedback](https://github.com/facebook/create-react-app/issues).
