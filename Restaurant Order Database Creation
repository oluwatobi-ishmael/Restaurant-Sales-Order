CREATE TABLE menu_items (
    menu_item_id SERIAL PRIMARY KEY,
    item_name VARCHAR(100) NOT NULL,
    category VARCHAR(50),
    price NUMERIC(10, 2) NOT NULL
);

CREATE TABLE order_details (
    order_details_id SERIAL PRIMARY KEY,
    order_id INTEGER NOT NULL,
    order_date DATE NOT NULL,
    order_time TIME NOT NULL,
    item_id INTEGER NOT NULL,
    FOREIGN KEY (item_id) REFERENCES menu_items(menu_item_id)
);

ALTER TABLE order_details
ALTER COLUMN item_id DROP NOT NULL;
