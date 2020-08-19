# LTV_project
Analyse the data set related to LTV model  with test: train.csv, test.csv, sample_submission.csv

Explanation of the data set:

The files contain randomized data about the behaviour and spending patterns of the
customers. It is used a similar data set to model the amount a user will spend during his
membership on the websites. This metric is called customer lifetime value (LTV).
The training set data are from users that have joined the website from Dec/2018
through June/2019. The test set contains users that joined in July/2019.
The data set contains the following columns:
- product_type: one of 4 different product_type a user can purchase. The user
always gets a first product (called ‘type_p’) and then can purchase additional
products (of ‘type_x’, ‘type_u’, and ‘type_ex’).
- user_id: a numerical identifier of the user. Note that for every user we might
have up to 4 rows, for the different product types.
- join_date: the moment when the user joined our site.
- hidden: a user segment estimated when joining our site according to available
data.
- product: the ‘type_p’ product that the user purchased when he joined.
- STV (short-term-value): the amount the user has spent on our sites in the first 4
days of his activity.
- target (lifetime value): the outcome variable. It is the amount the user has spent
after a little bit more than 2 months. This variable is only contained in the training
set.
- credit_card_level: one of two types of credit cards.
- is_lp: characterizes the traffic source.
- aff_type: another traffic source characterization.
- is_cancelled: did the user cancel his subscription for the respective
product_type within his first few days of activity?
- country_segment: from which country is the user?
The business model is a subscription based payment model. The users join the website
and pay a small amount for the first day. After one day, their subscription is converted to
a full amount (higher price) subscription, which is charged monthly. The user can also
request a refund, and we also have fraudulent users, which is why some target values
are negative.

The scope of this test is to understand the data provided and build a model in order to 
predict the LTV in the next month.
