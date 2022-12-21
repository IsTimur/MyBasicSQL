# MyBasicSQL

#CREATE VIEW vw_goods_and_goods_gategories AS
  SELECT g.id_goods,
         g.id_doods_category, 
         g.goods, 
         g.image, 
         g.brief_description, 
         g.price, 
         g.url_page, 
         c.id_categories
  FROM `goods` AS g
    INNER JOIN goods_categories AS c
        ON c.id_categories = g.id_categories;
