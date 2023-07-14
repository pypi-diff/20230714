# Comparing `tmp/ultima_scraper_db-0.1.0.tar.gz` & `tmp/ultima_scraper_db-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_db-0.1.0.tar", max compression
+gzip compressed data, was "ultima_scraper_db-0.1.1.tar", max compression
```

## Comparing `ultima_scraper_db-0.1.0.tar` & `ultima_scraper_db-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0    35149 2023-07-12 18:49:43.683779 ultima_scraper_db-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-07-12 18:49:43.683779 ultima_scraper_db-0.1.0/README.md
--rw-r--r--   0        0        0      632 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        1 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/databases/__init__.py
--rw-r--r--   0        0        0     5277 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/__init__.py
--rw-r--r--   0        0        0       58 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/alembic/README
--rw-r--r--   0        0        0     2694 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/alembic/env.py
--rw-r--r--   0        0        0      510 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/alembic/script.py.mako
--rw-r--r--   0        0        0    25993 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/alembic/versions/3ead48a37e21_.py
--rw-r--r--   0        0        0      911 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/alembic/versions/6d7d283707a8_.py
--rw-r--r--   0        0        0     3380 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/alembic.ini
--rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/schemas/__init__.py
--rw-r--r--   0        0        0     1958 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/schemas/management.py
--rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/schemas/templates/__init__.py
--rw-r--r--   0        0        0    21725 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/schemas/templates/site.py
--rw-r--r--   0        0        0     5840 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/helpers.py
--rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/managers/__init__.py
--rw-r--r--   0        0        0     8315 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/managers/database_manager.py
--rw-r--r--   0        0        0    25293 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/managers/site_db.py
--rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.0/ultima_scraper_db/py.typed
--rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 ultima_scraper_db-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-12 18:49:43.683779 ultima_scraper_db-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-12 18:49:43.683779 ultima_scraper_db-0.1.1/README.md
+-rw-r--r--   0        0        0      632 2023-07-14 09:05:02.845686 ultima_scraper_db-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.1/ultima_scraper_db/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.1/ultima_scraper_db/databases/__init__.py
+-rw-r--r--   0        0        0     5277 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/alembic/README
+-rw-r--r--   0        0        0     2694 2023-07-14 08:58:40.332193 ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/alembic/env.py
+-rw-r--r--   0        0        0      510 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/alembic/script.py.mako
+-rw-r--r--   0        0        0    26329 2023-07-14 08:56:39.528633 ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/alembic/versions/6ce7339b93e7_.py
+-rw-r--r--   0        0        0     3380 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/alembic.ini
+-rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/schemas/__init__.py
+-rw-r--r--   0        0        0     1958 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/schemas/management.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/schemas/templates/__init__.py
+-rw-r--r--   0        0        0    22236 2023-07-14 09:11:04.923038 ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/schemas/templates/site.py
+-rw-r--r--   0        0        0     4961 2023-07-14 05:31:36.252531 ultima_scraper_db-0.1.1/ultima_scraper_db/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.1/ultima_scraper_db/managers/__init__.py
+-rw-r--r--   0        0        0     8376 2023-07-14 08:56:18.849165 ultima_scraper_db-0.1.1/ultima_scraper_db/managers/database_manager.py
+-rw-r--r--   0        0        0    26519 2023-07-14 06:03:10.752821 ultima_scraper_db-0.1.1/ultima_scraper_db/managers/site_db.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.1.1/ultima_scraper_db/py.typed
+-rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 ultima_scraper_db-0.1.1/PKG-INFO
```

### Comparing `ultima_scraper_db-0.1.0/LICENSE` & `ultima_scraper_db-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.1.0/pyproject.toml` & `ultima_scraper_db-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-db"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["CRIMINAL <89371864+DIGITALCRIMINALS@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "ultima_scraper_db" }]
 include = ["ultima_scraper_db/py.typed"]
 
 [tool.poetry.dependencies]
```

### Comparing `ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/__init__.py` & `ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/alembic/env.py` & `ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/alembic/versions/3ead48a37e21_.py` & `ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/alembic/versions/6ce7339b93e7_.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 """empty message
 
-Revision ID: 3ead48a37e21
+Revision ID: 6ce7339b93e7
 Revises: 
-Create Date: 2023-07-10 04:11:03.771615
+Create Date: 2023-07-14 09:56:39.519642
 
 """
 from alembic import op
 import sqlalchemy as sa
 
 
 # revision identifiers, used by Alembic.
-revision = '3ead48a37e21'
+revision = '6ce7339b93e7'
 down_revision = None
 branch_labels = None
 depends_on = None
 
 
 def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
     op.create_table('media',
     sa.Column('id', sa.BigInteger(), autoincrement=False, nullable=False),
     sa.Column('url', sa.Text(), nullable=True),
     sa.Column('size', sa.BigInteger(), server_default='0', nullable=False),
-    sa.Column('category', sa.String(), nullable=False),
+    sa.Column('category', sa.String(), nullable=True),
     sa.Column('preview', sa.Boolean(), server_default='false', nullable=False),
     sa.Column('created_at', sa.TIMESTAMP(timezone=True), nullable=True),
     sa.PrimaryKeyConstraint('id'),
     schema='fansly'
     )
     op.create_table('users',
     sa.Column('id', sa.BigInteger(), autoincrement=False, nullable=False),
     sa.Column('username', sa.Text(), nullable=True),
     sa.Column('balance', sa.Float(), server_default='0', nullable=False),
     sa.Column('spend', sa.Boolean(), server_default='false', nullable=False),
     sa.Column('performer', sa.Boolean(), server_default='false', nullable=False),
+    sa.Column('favorite', sa.Boolean(), server_default='false', nullable=False),
     sa.Column('active', sa.Boolean(), server_default='true', nullable=False),
     sa.Column('downloaded_at', sa.TIMESTAMP(timezone=True), nullable=True),
     sa.Column('last_checked_at', sa.TIMESTAMP(timezone=True), nullable=True),
     sa.Column('join_date', sa.TIMESTAMP(timezone=True), nullable=True),
     sa.Column('created_at', sa.TIMESTAMP(timezone=True), server_default=sa.text("TIMEZONE('utc', CURRENT_TIMESTAMP)"), nullable=False),
     sa.Column('updated_at', sa.TIMESTAMP(timezone=True), nullable=True),
     sa.PrimaryKeyConstraint('id'),
@@ -64,26 +65,27 @@
     sa.PrimaryKeyConstraint('id'),
     schema='management'
     )
     op.create_table('media',
     sa.Column('id', sa.BigInteger(), autoincrement=False, nullable=False),
     sa.Column('url', sa.Text(), nullable=True),
     sa.Column('size', sa.BigInteger(), server_default='0', nullable=False),
-    sa.Column('category', sa.String(), nullable=False),
+    sa.Column('category', sa.String(), nullable=True),
     sa.Column('preview', sa.Boolean(), server_default='false', nullable=False),
     sa.Column('created_at', sa.TIMESTAMP(timezone=True), nullable=True),
     sa.PrimaryKeyConstraint('id'),
     schema='onlyfans'
     )
     op.create_table('users',
     sa.Column('id', sa.BigInteger(), autoincrement=False, nullable=False),
     sa.Column('username', sa.Text(), nullable=True),
     sa.Column('balance', sa.Float(), server_default='0', nullable=False),
     sa.Column('spend', sa.Boolean(), server_default='false', nullable=False),
     sa.Column('performer', sa.Boolean(), server_default='false', nullable=False),
+    sa.Column('favorite', sa.Boolean(), server_default='false', nullable=False),
     sa.Column('active', sa.Boolean(), server_default='true', nullable=False),
     sa.Column('downloaded_at', sa.TIMESTAMP(timezone=True), nullable=True),
     sa.Column('last_checked_at', sa.TIMESTAMP(timezone=True), nullable=True),
     sa.Column('join_date', sa.TIMESTAMP(timezone=True), nullable=True),
     sa.Column('created_at', sa.TIMESTAMP(timezone=True), server_default=sa.text("TIMEZONE('utc', CURRENT_TIMESTAMP)"), nullable=False),
     sa.Column('updated_at', sa.TIMESTAMP(timezone=True), nullable=True),
     sa.PrimaryKeyConstraint('id'),
@@ -103,28 +105,29 @@
     sa.Column('site_id', sa.BigInteger(), nullable=False),
     sa.Column('user_id', sa.BigInteger(), nullable=False),
     sa.Column('user_username', sa.Text(), nullable=False),
     sa.Column('category', sa.Text(), nullable=False),
     sa.Column('server_id', sa.BigInteger(), nullable=False),
     sa.Column('skippable', sa.Boolean(), server_default='false', nullable=False),
     sa.Column('active', sa.Boolean(), server_default='true', nullable=False),
+    sa.Column('completed_at', sa.TIMESTAMP(timezone=True), nullable=True),
     sa.ForeignKeyConstraint(['server_id'], ['management.servers.id'], ),
     sa.ForeignKeyConstraint(['site_id'], ['management.sites.id'], ),
     sa.ForeignKeyConstraint(['user_id'], ['fansly.users.id'], ),
     sa.PrimaryKeyConstraint('id'),
     sa.UniqueConstraint('site_id', 'user_id', 'category'),
     schema='fansly'
     )
     op.create_table('notifications',
     sa.Column('id', sa.Integer(), nullable=False),
     sa.Column('user_id', sa.BigInteger(), nullable=True),
     sa.Column('category', sa.String(), nullable=False),
     sa.Column('sent_discord', sa.Boolean(), server_default='false', nullable=False),
     sa.Column('sent_telegram', sa.Boolean(), server_default='false', nullable=False),
-    sa.Column('created_at', sa.TIMESTAMP(), server_default=sa.text("TIMEZONE('utc', CURRENT_TIMESTAMP)"), nullable=False),
+    sa.Column('created_at', sa.TIMESTAMP(timezone=True), server_default=sa.text("TIMEZONE('utc', CURRENT_TIMESTAMP)"), nullable=False),
     sa.ForeignKeyConstraint(['user_id'], ['fansly.users.id'], ),
     sa.PrimaryKeyConstraint('id'),
     schema='fansly'
     )
     op.create_table('socials',
     sa.Column('id', sa.Integer(), nullable=False),
     sa.Column('user_id', sa.BigInteger(), nullable=False),
@@ -245,28 +248,29 @@
     sa.Column('site_id', sa.BigInteger(), nullable=False),
     sa.Column('user_id', sa.BigInteger(), nullable=False),
     sa.Column('user_username', sa.Text(), nullable=False),
     sa.Column('category', sa.Text(), nullable=False),
     sa.Column('server_id', sa.BigInteger(), nullable=False),
     sa.Column('skippable', sa.Boolean(), server_default='false', nullable=False),
     sa.Column('active', sa.Boolean(), server_default='true', nullable=False),
+    sa.Column('completed_at', sa.TIMESTAMP(timezone=True), nullable=True),
     sa.ForeignKeyConstraint(['server_id'], ['management.servers.id'], ),
     sa.ForeignKeyConstraint(['site_id'], ['management.sites.id'], ),
     sa.ForeignKeyConstraint(['user_id'], ['onlyfans.users.id'], ),
     sa.PrimaryKeyConstraint('id'),
     sa.UniqueConstraint('site_id', 'user_id', 'category'),
     schema='onlyfans'
     )
     op.create_table('notifications',
     sa.Column('id', sa.Integer(), nullable=False),
     sa.Column('user_id', sa.BigInteger(), nullable=True),
     sa.Column('category', sa.String(), nullable=False),
     sa.Column('sent_discord', sa.Boolean(), server_default='false', nullable=False),
     sa.Column('sent_telegram', sa.Boolean(), server_default='false', nullable=False),
-    sa.Column('created_at', sa.TIMESTAMP(), server_default=sa.text("TIMEZONE('utc', CURRENT_TIMESTAMP)"), nullable=False),
+    sa.Column('created_at', sa.TIMESTAMP(timezone=True), server_default=sa.text("TIMEZONE('utc', CURRENT_TIMESTAMP)"), nullable=False),
     sa.ForeignKeyConstraint(['user_id'], ['onlyfans.users.id'], ),
     sa.PrimaryKeyConstraint('id'),
     schema='onlyfans'
     )
     op.create_table('socials',
     sa.Column('id', sa.Integer(), nullable=False),
     sa.Column('user_id', sa.BigInteger(), nullable=False),
```

### Comparing `ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/alembic.ini` & `ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/schemas/management.py` & `ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/schemas/management.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.1.0/ultima_scraper_db/databases/ultima/schemas/templates/site.py` & `ultima_scraper_db-0.1.1/ultima_scraper_db/databases/ultima/schemas/templates/site.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,68 +1,56 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, Any
 
 from sqlalchemy import (
-    TIMESTAMP,
     BigInteger,
     Boolean,
     Float,
     ForeignKey,
     Integer,
     SmallInteger,
     String,
     Text,
     UniqueConstraint,
     and_,
+    select,
 )
+from sqlalchemy.ext.asyncio import async_object_session
 from sqlalchemy.ext.compiler import compiles  # type: ignore
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from ultima_scraper_db.databases.ultima import (
     CustomFuncs,
     DefaultContentTypes,
     SiteTemplate,
 )
+from ultima_scraper_db.helpers import TIMESTAMPTZ, selectin_relationship
 
 if TYPE_CHECKING:
     from ultima_scraper_db.databases.ultima.schemas.management import SiteModel
 
 
-def selectin_relationship(*args: str, **kwargs: str):
-    return relationship(*args, lazy="selectin", **kwargs)
-
-
-def subquery_relationship(*args: str, **kwargs: str):
-    return relationship(*args, lazy="subquery", **kwargs)
-
-
 class UserModel(SiteTemplate):
     __tablename__ = "users"
 
     id: Mapped[int] = mapped_column(BigInteger, primary_key=True, autoincrement=False)
     username: Mapped[str] = mapped_column(Text, nullable=True)
     balance: Mapped[float] = mapped_column(Float, server_default="0")
     spend: Mapped[bool] = mapped_column(Boolean, server_default="false")
     performer: Mapped[bool] = mapped_column(Boolean, server_default="false")
     favorite: Mapped[bool] = mapped_column(Boolean, server_default="false")
     active: Mapped[bool] = mapped_column(Boolean, server_default="true")
-    downloaded_at: Mapped[datetime] = mapped_column(
-        TIMESTAMP(timezone=True), nullable=True
-    )
-    last_checked_at: Mapped[datetime] = mapped_column(
-        TIMESTAMP(timezone=True), nullable=True
-    )
-    join_date: Mapped[datetime | None] = mapped_column(
-        TIMESTAMP(timezone=True), nullable=True
-    )
+    downloaded_at: Mapped[datetime] = mapped_column(TIMESTAMPTZ, nullable=True)
+    last_checked_at: Mapped[datetime] = mapped_column(TIMESTAMPTZ, nullable=True)
+    join_date: Mapped[datetime | None] = mapped_column(TIMESTAMPTZ, nullable=True)
     created_at: Mapped[datetime] = mapped_column(
-        TIMESTAMP(timezone=True), server_default=CustomFuncs.utcnow()
+        TIMESTAMPTZ, server_default=CustomFuncs.utcnow()
     )
     updated_at: Mapped[datetime] = mapped_column(
-        TIMESTAMP(timezone=True), onupdate=CustomFuncs.utcnow(), nullable=True
+        TIMESTAMPTZ, onupdate=CustomFuncs.utcnow(), nullable=True
     )
     user_auth_info: Mapped["UserAuthModel"] = selectin_relationship()
     user_infos: Mapped[list["UserInfoModel"]] = relationship(
         foreign_keys="UserInfoModel.user_id", back_populates="user"
     )
 
     subscriptions: Mapped[list["SubscriptionModel"]] = relationship(
@@ -188,29 +176,48 @@
 
     async def find_bought_content(self, performer_id: int):
         await self.awaitable_attrs.bought_contents
         for bought_content in self.bought_contents:
             if bought_content.supplier_id == performer_id:
                 return bought_content
 
-    async def get_supplied_content(self):
+    async def get_supplied_content(self, active: bool = False):
+        final_supplied_content: list[BoughtContentModel] = []
         await self.awaitable_attrs.supplied_contents
-        return self.supplied_contents
+        if active:
+            for supplied_content in self.supplied_contents:
+                await supplied_content.awaitable_attrs.buyer
+                if not supplied_content.buyer.user_auth_info.active:
+                    continue
+                final_supplied_content.append(supplied_content)
+        else:
+            final_supplied_content = self.supplied_contents
+        return final_supplied_content
 
-    async def find_buyers(self):
+    async def find_buyers(self, active: bool = False):
         temp_buyers: set[UserModel] = set()
-        await self.awaitable_attrs.supplied_contents
-        for content in self.supplied_contents:
+        for content in await self.get_supplied_content(active=active):
             temp_buyers.add(await content.awaitable_attrs.buyer)
         await self.awaitable_attrs.subscribers
-        for subscription in self.subscribers:
-            # if subscription.expires_at < datetime.utcnow():
-            #     continue
-            temp_buyers.add(await subscription.awaitable_attrs.subscriber)  # type: ignore
-        return list(temp_buyers)
+        session = async_object_session(self)
+        assert session
+        query = (
+            select(UserModel)
+            .join(SubscriptionModel.subscriber)
+            .where(SubscriptionModel.user_id == self.id)
+        )
+        if active:
+            query = query.where(SubscriptionModel.expires_at >= datetime.now()).where(
+                UserModel.user_auth_info.has(active=True)
+            )
+        subscribers = await session.scalars(query)
+        for subscriber in subscribers:
+            temp_buyers.add(subscriber)
+        final_buyers = temp_buyers
+        return list(final_buyers)
 
     async def activate(self):
         self.user_auth_info.active = True
         await self.awaitable_attrs.subscriptions
         for subscription in self.subscriptions:
             await subscription.awaitable_attrs.user
             if subscription.user.active:
@@ -263,20 +270,16 @@
     image_count: Mapped[int] = mapped_column(Integer, server_default="0")
     video_count: Mapped[int] = mapped_column(Integer, server_default="0")
     audio_count: Mapped[int] = mapped_column(Integer, server_default="0")
     favourited_count: Mapped[int] = mapped_column(Integer, server_default="0")
     size: Mapped[int] = mapped_column(BigInteger, server_default="0")
     location: Mapped[str] = mapped_column(Text, nullable=True)
     website: Mapped[str] = mapped_column(Text, nullable=True)
-    downloaded_at: Mapped[datetime] = mapped_column(
-        TIMESTAMP(timezone=True), nullable=True
-    )
-    uploaded_at: Mapped[datetime] = mapped_column(
-        TIMESTAMP(timezone=True), nullable=True
-    )
+    downloaded_at: Mapped[datetime] = mapped_column(TIMESTAMPTZ, nullable=True)
+    uploaded_at: Mapped[datetime] = mapped_column(TIMESTAMPTZ, nullable=True)
     user: Mapped["UserModel"] = relationship(back_populates="user_infos")
 
 
 class ContentMediaAssoModel(DefaultContentTypes, SiteTemplate):
     __tablename__ = "content_media_asso"
     __table_args__ = (
         UniqueConstraint("story_id", "post_id", "message_id", "media_id"),
@@ -312,15 +315,15 @@
 class MediaModel(SiteTemplate):
     __tablename__ = "media"
     id: Mapped[int] = mapped_column(BigInteger, primary_key=True, autoincrement=False)
     url: Mapped[str] = mapped_column(Text, nullable=True)
     size: Mapped[int] = mapped_column(BigInteger, server_default="0", default="0")
     category: Mapped[str] = mapped_column(String, nullable=True)
     preview: Mapped[bool] = mapped_column(Boolean, server_default="false")
-    created_at: Mapped[datetime | None] = mapped_column(TIMESTAMP(timezone=True))
+    created_at: Mapped[datetime | None] = mapped_column(TIMESTAMPTZ)
     filepaths: Mapped[list["FilePathModel"]] = relationship(
         "FilePathModel",
         # back_populates="media",
     )
 
     content_media_assos: Mapped[list[ContentMediaAssoModel]] = relationship(
         back_populates="media"
@@ -342,15 +345,15 @@
 
 
 class StoryModel(ContentTemplate):
     __tablename__ = "x_stories"
 
     id: Mapped[int] = mapped_column(BigInteger, primary_key=True, autoincrement=False)
     user_id: Mapped[int] = mapped_column(BigInteger, ForeignKey("users.id"))
-    created_at: Mapped[datetime] = mapped_column(TIMESTAMP(timezone=True))
+    created_at: Mapped[datetime] = mapped_column(TIMESTAMPTZ)
 
     user: Mapped["UserModel"] = relationship(
         foreign_keys=user_id,
     )
 
     media: Mapped[list["MediaModel"]] = relationship(
         "MediaModel",
@@ -375,15 +378,15 @@
     id: Mapped[int] = mapped_column(BigInteger, primary_key=True, autoincrement=False)
     user_id: Mapped[int] = mapped_column(BigInteger, ForeignKey("users.id"))
     text: Mapped[str] = mapped_column(Text, nullable=True)
     price: Mapped[float] = mapped_column(Float, server_default="0")
     deleted: Mapped[bool] = mapped_column(Boolean, server_default="false")
     archived: Mapped[bool] = mapped_column(Boolean, server_default="false")
     paid: Mapped[bool | None] = mapped_column(Boolean, nullable=True)
-    created_at: Mapped[datetime] = mapped_column(TIMESTAMP(timezone=True))
+    created_at: Mapped[datetime] = mapped_column(TIMESTAMPTZ)
 
     user: Mapped["UserModel"] = relationship(
         foreign_keys=user_id,
     )
 
     media: Mapped[list["MediaModel"]] = relationship(
         "MediaModel",
@@ -411,15 +414,15 @@
         BigInteger, ForeignKey("users.id"), nullable=True
     )
     text: Mapped[str] = mapped_column(Text, nullable=True)
     price: Mapped[float] = mapped_column(Float, server_default="0")
     deleted: Mapped[bool] = mapped_column(Boolean, server_default="false")
     paid: Mapped[bool | None] = mapped_column(Boolean, nullable=True)
     verified: Mapped[bool] = mapped_column(Boolean, server_default="false")
-    created_at: Mapped[datetime] = mapped_column(TIMESTAMP(timezone=True))
+    created_at: Mapped[datetime] = mapped_column(TIMESTAMPTZ)
 
     user: Mapped["UserModel"] = relationship(
         foreign_keys=user_id,
     )
     media: Mapped[list["MediaModel"]] = relationship(
         "MediaModel",
         secondary=ContentMediaAssoModel.__table__,
@@ -444,30 +447,28 @@
     reply_id: Mapped[int] = mapped_column(
         BigInteger, ForeignKey("comments.id"), nullable=True
     )
     user_id: Mapped[int] = mapped_column(BigInteger)
     giphy_id: Mapped[str | None] = mapped_column(String, server_default=None)
     text: Mapped[str | None] = mapped_column(String, server_default=None)
     likes_count: Mapped[int] = mapped_column(Integer, server_default="0")
-    created_at: Mapped[datetime] = mapped_column(TIMESTAMP(timezone=True))
+    created_at: Mapped[datetime] = mapped_column(TIMESTAMPTZ)
 
 
 class SubscriptionModel(SiteTemplate):
     __tablename__ = "subscriptions"
     __table_args__ = (UniqueConstraint("user_id", "subscriber_id"),)
 
     id: Mapped[int] = mapped_column(primary_key=True)
     user_id: Mapped[int] = mapped_column(BigInteger, ForeignKey("users.id"))
     subscriber_id: Mapped[int] = mapped_column(BigInteger, ForeignKey("users.id"))
     paid_content: Mapped[bool] = mapped_column(Boolean, server_default="0")
     active: Mapped[bool] = mapped_column(Boolean, server_default="true")
-    downloaded_at: Mapped[datetime] = mapped_column(
-        TIMESTAMP(timezone=True), nullable=True
-    )
-    expires_at: Mapped[datetime] = mapped_column(TIMESTAMP(timezone=True))
+    downloaded_at: Mapped[datetime] = mapped_column(TIMESTAMPTZ, nullable=True)
+    expires_at: Mapped[datetime] = mapped_column(TIMESTAMPTZ)
 
     user: Mapped["UserModel"] = relationship(
         "UserModel",
         foreign_keys="SubscriptionModel.user_id",
     )
     subscriber: Mapped["UserModel"] = relationship(
         "UserModel",
@@ -528,29 +529,30 @@
     user_username: Mapped[str] = mapped_column(Text)
     category: Mapped[str] = mapped_column(Text)
     server_id: Mapped[int] = mapped_column(
         BigInteger, ForeignKey("management.servers.id")
     )
     skippable: Mapped[bool] = mapped_column(Boolean, server_default="false")
     active: Mapped[bool] = mapped_column(Boolean, server_default="true")
+    completed_at: Mapped[datetime | None] = mapped_column(TIMESTAMPTZ, nullable=True)
     user: Mapped[UserModel] = relationship(back_populates="jobs")
     site: Mapped["SiteModel"] = relationship(foreign_keys=site_id)
 
 
 class NotificationModel(SiteTemplate):
     __tablename__ = "notifications"
     id: Mapped[int] = mapped_column(primary_key=True)
     user_id: Mapped[int] = mapped_column(
         BigInteger, ForeignKey("users.id"), nullable=True
     )
     category: Mapped[str] = mapped_column(String)
     sent_discord: Mapped[bool] = mapped_column(Boolean, server_default="false")
     sent_telegram: Mapped[bool] = mapped_column(Boolean, server_default="false")
     created_at: Mapped[datetime] = mapped_column(
-        TIMESTAMP, server_default=CustomFuncs.utcnow()
+        TIMESTAMPTZ, server_default=CustomFuncs.utcnow()
     )
 
     user: Mapped["UserModel"] = selectin_relationship()
 
 
 class SocialModel(SiteTemplate):
     __tablename__ = "socials"
@@ -566,10 +568,7 @@
 
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
     supplier_id: Mapped[int] = mapped_column(BigInteger, ForeignKey("users.id"))
     buyer_id: Mapped[int] = mapped_column(BigInteger, ForeignKey("users.id"))
 
     supplier: Mapped[UserModel] = relationship(foreign_keys=supplier_id)
     buyer: Mapped[UserModel] = relationship(foreign_keys=buyer_id)
-
-
-# REMOVE
```

### Comparing `ultima_scraper_db-0.1.0/ultima_scraper_db/helpers.py` & `ultima_scraper_db-0.1.1/ultima_scraper_db/helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import sqlalchemy as sa
 from sqlalchemy.exc import OperationalError, ProgrammingError
 from sqlalchemy.ext.asyncio import AsyncEngine, create_async_engine
+from sqlalchemy.orm import relationship
 from sqlalchemy_utils.functions.database import _set_url_database  # type: ignore
 from sqlalchemy_utils.functions.database import _sqlite_file_exists  # type: ignore
 from sqlalchemy_utils.functions.database import make_url  # type: ignore
 from sqlalchemy_utils.functions.orm import quote  # type: ignore
-from ultima_scraper_api import user_types
-from ultima_scraper_api.apis.onlyfans.classes.user_model import (
-    create_user as OFUserModel,
-)
 
-from ultima_scraper_db.databases.ultima.schemas.templates.site import UserModel
+TIMESTAMPTZ = sa.TIMESTAMP(timezone=True)
+
+
+def selectin_relationship(*args: str, **kwargs: str):
+    return relationship(*args, lazy="selectin", **kwargs)
+
+
+def subquery_relationship(*args: str, **kwargs: str):
+    return relationship(*args, lazy="subquery", **kwargs)
 
 
 async def _get_scalar_result(engine: AsyncEngine, sql: sa.TextClause):
     try:
         async with engine.connect() as conn:
             return await conn.scalar(sql)
     except Exception as _e:
@@ -118,35 +123,7 @@
 
     else:
         async with engine.begin() as conn:
             text = f"CREATE DATABASE {quote(conn, database)}"
             await conn.execute(sa.text(text))
 
     await engine.dispose()
-
-
-async def is_valuable(user: UserModel | user_types):
-    # Checks if performer has active subscription or has supplied content to a buyer
-    # We can add a "valid flag on get_supplied_content to return active authed users"
-    if isinstance(user, UserModel):
-        if await user.has_active_subscription() or await user.get_supplied_content():
-            return True
-        else:
-            return False
-    else:
-        if user.isPerformer:
-            if isinstance(user, OFUserModel):
-                if (
-                    user.subscribedIsExpiredNow == False
-                    or await user.get_paid_contents()
-                ):
-                    return True
-                else:
-                    return False
-            else:
-                # We need to add paid_content checker
-                if user.following:
-                    return True
-                else:
-                    return False
-        else:
-            return False
```

### Comparing `ultima_scraper_db-0.1.0/ultima_scraper_db/managers/database_manager.py` & `ultima_scraper_db-0.1.1/ultima_scraper_db/managers/database_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,17 @@
 
         async with self.engine.connect() as conn:
             current_rev = await conn.run_sync(get_current_revision)
             assert self.alembica
             alembic_cfg = self.alembica.config
             if not current_rev:
                 try:
-                    _revision = await conn.run_sync(run_revision, alembic_cfg, True)
+                    _revision = await conn.run_sync(
+                        run_revision, alembic_cfg, True, self.metadata
+                    )
                     pass
                 except CommandError as _e:
                     await self.run_migrations()
                     pass
             else:
                 _revision = await conn.run_sync(
                     run_revision, alembic_cfg, True, self.metadata
```

### Comparing `ultima_scraper_db-0.1.0/ultima_scraper_db/managers/site_db.py` & `ultima_scraper_db-0.1.1/ultima_scraper_db/managers/site_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,56 +8,58 @@
 from sqlalchemy.sql import and_, exists, select, union_all
 from ultima_scraper_api.apis.onlyfans.classes.comment_model import (
     CommentModel as OFCommentModel,
 )
 from ultima_scraper_api.apis.onlyfans.classes.user_model import (
     create_user as OFUserModel,
 )
+from ultima_scraper_collection.helpers.main_helper import is_valuable
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
     ContentMetadata,
 )
-
 from ultima_scraper_db.databases.ultima.schemas.templates.site import (
     BoughtContentModel,
     CommentModel,
     FilePathModel,
     MediaModel,
     MessageModel,
     NotificationModel,
     PostModel,
     StoryModel,
     SubscriptionModel,
     UserAuthModel,
     UserInfoModel,
     UserModel,
 )
-from ultima_scraper_db.helpers import is_valuable
 from ultima_scraper_db.managers.database_manager import Schema
 
 content_model_types = StoryModel | PostModel | MessageModel
 from ultima_scraper_api import post_types
 
 if TYPE_CHECKING:
     from ultima_scraper_collection import datascraper_types
 
 
 class ContentManager:
     def __init__(
         self,
         user: "UserModel",
     ):
-        self.stories: list["StoryModel"] = user._stories  # type: ignore
-        self.posts: list["PostModel"] = user._posts  # type: ignore
-        self.messages: list["MessageModel"] = user._messages  # type: ignore
         self.__user__ = user
 
-    async def get_contents(self, content_type: str | None = None):
+    async def init(self):
         await self.__user__.awaitable_attrs._stories
         await self.__user__.awaitable_attrs._posts
         await self.__user__.awaitable_attrs._messages
+        self.stories: list["StoryModel"] = self.__user__._stories  # type: ignore
+        self.posts: list["PostModel"] = self.__user__._posts  # type: ignore
+        self.messages: list["MessageModel"] = self.__user__._messages  # type: ignore
+        return self
+
+    async def get_contents(self, content_type: str | None = None):
         if content_type:
             # if not hasattr(self, content_type.lower()):
             #     empty_list: content_model_types = []
             #     return empty_list
             result: list[content_model_types] = getattr(self, content_type.lower())
             return result
         return self.stories + self.posts + self.messages
@@ -175,14 +177,45 @@
         result2 = await session.execute(stmt2)
         result3 = await session.execute(stmt3)
         final_sum = sum(
             (result1.scalar() or 0, result2.scalar() or 0, result3.scalar() or 0)
         )
         return final_sum
 
+    async def media_sum(self, category: str):
+        session = async_object_session(self.__user__)
+        assert session
+
+        stmt1 = (
+            select(func.count())
+            .where(MediaModel.category == category)
+            .where(MediaModel.filepaths.any())
+            .join(StoryModel.media)
+            .where(StoryModel.user_id == self.__user__.id)
+        )
+        stmt2 = (
+            select(func.count())
+            .where(MediaModel.category == category)
+            .where(MediaModel.filepaths.any())
+            .join(PostModel.media)
+            .where(PostModel.user_id == self.__user__.id)
+        )
+        stmt3 = (
+            select(func.count())
+            .where(MediaModel.category == category)
+            .where(MediaModel.filepaths.any())
+            .join(MessageModel.media)
+            .where(MessageModel.user_id == self.__user__.id)
+        )
+        result1 = await session.scalar(stmt1)
+        result2 = await session.scalar(stmt2)
+        result3 = await session.scalar(stmt3)
+        final_sum = sum((result1 or 0, result2 or 0, result3 or 0))
+        return final_sum
+
 
 class StatementBuilder:
     def __init__(self, model: Type[UserModel | UserInfoModel]) -> None:
         self.model = model
         self.statement: Select[Any] = select(model)
 
     def filter_by_user_identifiers(self, identifiers: list[int | str]):
@@ -347,15 +380,15 @@
         _s = await db_user.awaitable_attrs._stories
         _p = await db_user.awaitable_attrs._posts
         _m = await db_user.awaitable_attrs._messages
         pass
         for _key, contents in api_user.content_manager.categorized.__dict__.items():
             for _, content in contents.items():
                 await self.create_or_update_content(db_user, content)
-        db_user.last_checked_at = datetime.utcnow()
+        db_user.last_checked_at = datetime.now()
         user_info.size = await db_user.content_manager.sum()
         await self.session.flush()
         return db_user
 
     async def create_or_update_auth_info(
         self, api_authed: ultima_scraper_api.auth_types, db_user: UserModel
     ):
@@ -444,15 +477,15 @@
         return user_info
 
     async def create_or_update_content(
         self, db_performer: UserModel, content: ContentMetadata
     ):
         api_performer = content.__soft__.get_author()
         api_type = content.api_type
-        content_manager = db_performer.content_manager
+        content_manager = await db_performer.content_manager.init()
         found_db_content = await content_manager.find_content(content.content_id)
         if not found_db_content:
             pass
         if content.paid:
             pass
         db_content = found_db_content or await content_manager.add_content(content)
         db_content_paid = None
```

### Comparing `ultima_scraper_db-0.1.0/PKG-INFO` & `ultima_scraper_db-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-db
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: CRIMINAL
 Author-email: 89371864+DIGITALCRIMINALS@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

